## Core Stack
A base stack built on top of Laravel. 

## System Requirements
- PHP (https://www.php.net/downloads.php)
- Composer (https://getcomposer.org/download/)
- Docker (https://docs.docker.com/get-docker/)
- NodeJs (https://nodejs.org/en/download/)

## Installation
The installation process assumes you have PHP, Node, Composer and Docker globally installed. 

- Bring the code locally `git clone git@github.com:Lopez-Global/dataServices.git`
- Install the required libraries `composer install`
- Rename `.env.example` to `.env`
- Create an application key `php artisan key:generate`
- Run sails `php artisan sail:install` then setup mariadb, redis, mailhog, selenium `2,3,7,8`
- Build the docker containers and run them `docker-compose up -d` 

## Migrations
There is a bug when running migrations when using docker. 
- In your .env file, change `DB_HOST=mariadb` to `DB_HOST=localhost`. 
- Run the database migrations `php artisan migrate`
- Change the .env file back to `DB_HOST=mariadb`

