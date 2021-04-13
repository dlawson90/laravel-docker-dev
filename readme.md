# Basic Docker Dev Environment for Laravel

Basic local dev environment using docker, for use with Laravel.

## Commands

---
`docker-compose pull`

`docker-compose build`

`docker-compose up -d`

`docker-compose down`

## Notes

---
### mysql

Setting MYSQL_USER and MYSQL_PASSWORD will create a new user, but won't have ALL PRIVILEGES. This needs to be set from within phpmyadmin.

| Env Key             | Description                       | 
| ------------------- | --------------------------------- |
| MYSQL_DATABASE      | database name (must match env)    |
| MYSQL_ROOT_PASSWORD | password for root user            |
| MYSQL_USER          | username for user that's created  |
| MYSQL_PASSWORD      | password for user that's created  |


### phpmyadmin
| Env Key      | Description                        |
| ------------ | ---------------------------------- |
| PMA_HOST     | database service name              |
| PMA_USER     | user (for auto login purposes)     |
| PMA_PASSWORD | password (for auto login purposes) |
