#### Step 1: Build MySQL Docker Image
```sh
docker build -t codspire/mysql .
```

#### Step 2: Run MySQL Docker Container
```sh
docker run --name mysql-container -d -p 3306:3306 codspire/mysql
```

#### Step 3: Check Container Status
```sh
docker ps
```

#### Step 4: ssh to database container
```sh
docker exec -i -t mysql-container bash
```

#### Step 5: Connect to MySQL database
```sh
mysql -uroot -ppassword
```
