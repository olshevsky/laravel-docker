# Minimalistic docker setup for Laravel 9
Alpine based docker setup for Laravel 9.

## Setup includes:
* nginx:1.20.2-alpine
* php:8.1-fpm-alpine
* mysql:5.7.37
* phpmyadmin

## Php extensions: 
bcmath
Core
ctype
curl
date
dom
fileinfo
filter
ftp
hash
iconv
json
libxml
mbstring
mysqlnd
openssl
pcre
PDO
pdo_mysql
pdo_sqlite
Phar
posix
readline
Reflection
session
SimpleXML
sodium
SPL
sqlite3
standard
tokenizer
xml
xmlreader
xmlwriter
zlib

## Installation:
1. Copy files from this repo into your Laravel project (replacing original docker-compose.yml)
2. Rename .env.example to .env and edit it. Note that ***DB_HOST in .env must match DB service name in docker-compose.yml*** (e.g. DB_HOST=mysql)
3. In project directory run:
```
docker-compose -p {project-name} up -d
```

## App url:
http://localhost:80/

## phpMyAdmin url:
http://localhost:8080/
