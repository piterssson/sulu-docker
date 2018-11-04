# Sulu-Docker


## Instalation


### First build docker

```
docker-compose build
docker-compose up -d
```

### Second install sulu

```
mkdir src (linux)
docker-compose exec php bash
composer create-project "sulu/sulu-minimal" .
composer install
```


##### File app/config/parameters.yml :

```
parameters:
    database_driver: pdo_mysql
    database_host: db
    database_port: 3306
    database_name: sulu
    database_user: sulu
    database_password: sulu
    database_version: 5.7
```