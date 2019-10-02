# RESTful API Development with PHPSymfony 4.2
This project demonstrate on how to develop RESTful API application with CRUD method using PHP Symfony 4.2 framework and PHP version 7.2.10, under docker container environment.

So, make sure you have installed docker and docker-compose ready on your environment. Then, you can follow the setup guide step by step.

## Setup Guide
* git clone git@gitlab.com:plutosolutions/php-symfony4-web-api-appication.git
* cd PHP-Symfony4-Web-API-Application
* docker-compose build
* docker-compose up -d
* docker-compose exec php bash
	* cd symfony
	* composer install
	* php bin/console doctrine:database:create
	* php bin/console doctrine:migrations:migrate
* API Endpoint http://localhost:5031/api

## CRUD API
* POST http://localhost:5031//api/users
* GET http://localhost:5031//api/users
* GET http://localhost:5031//api/users/{id}
* PUT http://localhost:5031//api/users/{id}
* DELETE http://localhost:5031//api/users/{id}

## Example POST Data
```
{
   "username":"username#1",
   "userpassword": "A3450%^&*"
}
```
