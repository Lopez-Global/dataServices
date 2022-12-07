## Core Stack
A base stack built on top of Laravel. 

## Installation

- Bring the code locally `git clone git@github.com:Lopez-Global/dataServices.git`
- Install the required libraries `composer install`
- Rename `.env.example` to `.env`
- Run sails `php artisan sail:install` then setup mariadb, redis, mailhog, selenium `2,3,7,8`
- In your .env file, change `DB_HOST` to `DB_HOST=localhost`. This is due to a bug with the way the DB hostname is exposed to your system. 
- Build the docker containers and run them `docker-compose up -d` 
