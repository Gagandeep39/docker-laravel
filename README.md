# Laravel Application

- [Laravel Application](#laravel-application)
  - [MYSQL](#mysql)
  - [Server](#server)
  - [Composer](#composer)
  - [Steps Executed](#steps-executed)

## MYSQL

- Used to store persistent data

## Server

- Nginx server used to deploy Server code

## Composer

- Used to create laravel project
- Similar to npm used by nodejs
- Saves us from natively installing composer package

## Steps Executed

1. Created Utility docker files
2. Created environment files
3. Created nginx conf file
4. Created docker-compose file
5. Execute `docker-compose run --rm composer create-project --prefer-dist laravel/laravel .` to create laravel project
