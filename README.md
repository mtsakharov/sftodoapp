Symfony4 Todo App
========

A Symfony 4 project, with an API skeleton using JWT for user authentication.

## Installation


`docker-compose build`

`docker-compose up -d`

`docker-compose exec php-fpm bash`

`composer install`

#### Configuration Parameters

You may add the default ones given by hitting enter (as the values are set by Docker config), except for the **mailer parameters**, please update those with your mailer provider.

#### Creating the database schema

You can do this by running the script, which will create a clean database and schema.

`bash install-clean.sh`

#### Fixtures

If you want to create the database with some fixtures, you may run the script 

`bash install-import-fixtures.sh`

## Docker

To run the application in development mode

`docker-compose up -d`

## Clear Cache

Shell into the PHP container

`docker-compose exec php-fpm bash`

To clear the cache, run the script with the environment parameter

`bash cacl.sh prod`

`bash cacl.sh dev`

## Tests
Shell into the PHP container

`docker-compose exec php-fpm bash`

Then run the script to run tests without debug

`bash runtests.sh`

Include 'debug' parameter to run with debug

`bash runtests.sh debug`



