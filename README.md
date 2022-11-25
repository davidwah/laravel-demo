# Travellist - Laravel Demo App

This is a Laravel demo application to support our Laravel guides.


## Setting Up the Application’s `.env` File
```
nano .env
```
## Setting Up the Application’s Dockerfile
```
nano Dockerfile
```
## Setting Nginx Configuration and Database Dump File
```
mkdir -p docker-compose/nginx

nano docker-compose/nginx/travellist.conf

mkdir docker-compose/mysql

nano docker-compose/mysql/init_db.sql
```
## Creating a Multi-Container Environment with Docker Compose
```
nano docker-compose.yml
```
## Running the Application with Docker Compose
```
docker-compose build app

docker-compose up -d

docker-compose ps

docker-compose exec app ls -l

docker-compose exec app rm -rf vendor composer.lock
docker-compose exec app composer install

docker-compose exec app php artisan key:generate
```
## Access Web Application on Browser
[http://localhost:8000](http://localhost:8000)
