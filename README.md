# RESTful API with PHP Symfony 4.2
This project demonstrate on how to develop RESTful API application with CRUD method using PHP Symfony 4.2 framework and PHP version 7.2.10, under docker container environment.

So, make sure you have installed docker and docker-compose ready on your environment. Then, you can follow the setup guide step by step.

## Stack
* PHP 7.2, Symfony 4.2
* MySQL
* docker/docker-compose

## Setup Guide
* git clone https://github.com/Khachornchit/PHP-Symfony4-RESTful-API.git
* cd PHP-Symfony4-RESTful-API
* docker-compose build
* docker-compose up -d
* docker-compose exec php bash
	* cd symfony
	* composer install
	* php bin/console doctrine:database:create
	* php bin/console doctrine:migrations:migrate

## API Endpoint
* http://localhost:5031/api

## Sample CRUD
* POST		/users
* GET		/users
* GET		/users/{id}
* PUT		/users/{id}
* DELETE	/users/{id}

## Data
```
{
   "username":"username#1",
   "userpassword": "A3450%^&*"
}
```
