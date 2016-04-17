#### Step 1: Build MySQL Docker Image
```sh
$ docker build -t codspire/mysql .
```

#### Step 2: Run MySQL Docker Container
```sh
$ docker run --name mysql-container -d -p 3306:3306 codspire/mysql
```

#### Step 3: Check Container Status
```sh
$ docker ps
```

#### Step 4: ssh to Database Container
```sh
$ docker exec -i -t mysql-container bash
```

#### Step 5: Connect to MySQL Database (command prompt)
```sh
$ mysql -uroot -ppassword

mysql> show schemas;

mysql> desc db;

mysql> desc event;

mysql> desc user;

mysql> select user from user;
```
Note: MySQL is case sensitive.

#### or
#### Connect Using Database Client (e.g. SQuirrel SQL Client)

`$ docker-machine ip default`

Will return the Container IP addess

Create new Connection in SQL Client using

**URL** = `jdbc:mysql://<IP Address>:3306/mysql`

**User Name** = `root`

**Password** = `password`

