# User-details-API-Nodejs-Mysql
A simple Login/Register application developed in Nodejs using Express.

# Getting started

Unzip the downloaded file.

### Installing dependencies:
Enter this command it will install all the dependencies at once:

```
npm install
```
Or you can install them individually:

```
npm install express express-session mysql pug-cli bcrypt util.promisify
```

Sometimes you get errors and access denied add sudo to the command

```
sudo npm install express express-session mysql pug-cli bcrypt util.promisify
```

### Start the application

```
npm start
```
or
```
node app
```
### Database

For this application the database  name is 'www', it contains only one table 'users'

Go to core/pool.js enter your database username and password, you can use you own database name just make sure it's the same in the pool.js file so you can connect to database.

### Setting up the database

You can use PhpMyAdmin just import the database.sql file includes in the project directory

Use those queries:

```
CREATE DATABASE www;
```
```
USE www;
```


if you correcty setting up the database you shouldn't get any errors.

```
Task:4
'SQL Assignment'
SELECT a.cname AS "Customer Name", 
a.city, b.name AS "Salesman", b.city,b.commission  
FROM customer a  
INNER JOIN salesman b  
ON a.salesman_id=b.salesman_id 
WHERE b.commission>.12 
AND a.city<>b.city;

```
