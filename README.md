## Core Stack
A base stack built on top of Laravel. 

## Installation

- Bring the code locally `git clone git@github.com:dlopez/coreStack.git`
- Install the required libraries `composer install`
- Build the docker containers and run them `docker-compose up -d` 
- In your .env file, change `DB_HOST` to `DB_HOST=localhost`. This is due to a bug with the way the DB hostname is exposed to your system. 