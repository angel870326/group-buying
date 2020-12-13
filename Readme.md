### Clone

Clone this repository to your local machine

```
$ git clone 
```

### Setup Datebase

**Create and use group_buying MySQL database**

> Run the following code
```
drop database if exists group_buying;
create database group_buying;
use group_buying;
```

### Setup App

**Enter the project folder**

```
$ cd group_buying
```

**Install packages via npm**

```
$ npm install
```

**Edit password in config.json file**

> /config/config.json
```
"development": {
  "username": "root",
  "password": "<YOUR_WORKBENCH_PASSWORD>",
  "database": "group_buying",
  "host": "127.0.0.1",
  "dialect": "mysql",
  "operatorsAliases": false
}

```

**Create models**

> run the following code in the console
```
$ npx sequelize db:migrate
```

**Activate the server**

```
$ npm run dev
```

**Find the message for successful activation**

```
> App is running on port 3000!
```
You may visit the application on browser with the URL: http://localhost:3000