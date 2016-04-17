#### Step 1: Add DB connection details in the pom file
`<url>**jdbc:mysql://<hostname/IP address>:3306/**</url>`

Get container IP address by running `docker-machine ip default`

mvn clean package flyway:baseline flyway:migrate flyway:info
