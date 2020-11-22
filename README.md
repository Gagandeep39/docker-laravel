# Laravel Application

- [Laravel Application](#laravel-application)
  - [MYSQL](#mysql)
  - [Server](#server)
  - [Composer](#composer)
  - [artisan](#artisan)
  - [Steps Executed](#steps-executed)

## MYSQL

- Used to store persistent data

## Server

- Nginx server used to deploy Server code

## Composer

- Used to create laravel project
- Similar to npm used by nodejs
- Saves us from natively installing composer package

## artisan

- Used by laravel
- Populates database with some dummy data iitially
- Works with same dockerfile as php

## Steps Executed

1. Created Utility docker files
2. Created environment files
3. Created nginx conf file
4. Created docker-compose file
5. Execute `docker-compose run --rm composer create-project --prefer-dist laravel/laravel .` to create laravel project
6. Start specific services `docker-compose up --build mysql server php`
7. Tried accessing `localhost:8000` in browser (Everything works)
8. Added artisan and npm service in docker-compose
9. Add dummy data in tables `docker-compose run --rm artisan migrate`
10. Created a nginx, php docker file for production
11. Created dodcker-compose for production
12. `docker-compose -f docker-compose.prod.yml up --build server`
