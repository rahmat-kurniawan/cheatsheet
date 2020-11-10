# Adonis Cheatsheet
## Install Adonis
```
npm install -g @adonisjs/cli 
```
## Creating App Api-Only
```
adonis new schedulerapi --api-only
```
## Run App
```
adonis serve --dev
```
## Add Database
```
npm i --save mysql

npm i --save pg

npm i --save sqlite3
```
## Config Databases
```
DB_CONNECTION = [mysql, sqlite, pg]
DB_HOST = YOUR_LOCALHOST_ADDRESS
DB_PORT = YOUR_PORT
DB_USER = YOUR_DB_USER
DB_PASSWORD = YOUR_DB_PASSWORD
DB_DATABASE= YOUR_DATABASE_NAME
```
## Create Migration
```
adonis make:migration users
```
## Migration
```
adonis migration:run
```
## Create Controller
```
adonis make:controller User
adonis make:controller UpdateUserInfo --type http
```