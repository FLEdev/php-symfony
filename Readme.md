# Description
## This Bundle contains split approach for Backend and Frontend Application.
## Backend = Symfony served via Symfony CLI

# Prerequisites
## PHP
## Symfony CLI: https://symfony.com/doc/current/setup/symfony_cli.html
## NodeJs

# Installation
## $ brew install symfony-cli/tap/symfony-cli
## $ symfony server:ca:install
## $ composer install

# Schema
## php bin/console doctrine:schema:validate
## php bin/console doctrine:schema:update --force

# Start
## $ php bin/console doctrine:fixtures:load
## $ symfony server:start -d
## $ pnpm run dev --turbopack

# Url
## BE: http://127.0.0.1:8000
## FE: http://127.0.0.1:3000


# Stop
## $ symfony server:stop
## $ symfony server:log

# Commands used
$ composer create-project symfony/skeleton:"8.0.*" .
$ composer require --dev symfony/maker-bundle symfony/debug-bundle symfony/maker-bundle doctrine/doctrine-fixtures-bundle
$ composer require symfony/orm-pack symfony/validator symfony/serializer api lexik/jwt-authentication-bundle 

$ php bin/console doctrine:schema:create
$ php bin/console doctrine:schema:validate
$ php bin/console list doctrine
$ 
$ php bin/console dbal:run-sql 'SELECT * FROM product'
$
$ php bin/console doctrine:generate:entity


$ symfony server:start -d


# ToDo
## Add Authentification and Authorization
## Add Nemlio (OpenAPI / SwaggerUI): https://symfony.com/bundles/NelmioApiDocBundle/current/index.html







