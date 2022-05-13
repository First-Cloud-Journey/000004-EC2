# AWS-FCJ-Management - Nodejs, Express, MySQL & Handlebars

### Demo

1. **Homepage**

![Homepage](https://github.com/Van-Hoang-Kha/AWS-FCJ-Management/blob/master/images/homepage.png)

2. **View User**

![Viewuser](https://github.com/Van-Hoang-Kha/AWS-FCJ-Management/blob/master/images/viewuser.png)

3. **Add User**

![Add user](https://github.com/Van-Hoang-Kha/AWS-FCJ-Management/blob/master/images/adduser.png)

4. **Edit User**

![Edituser](https://github.com/Van-Hoang-Kha/AWS-FCJ-Management/blob/master/images/edituser.png)

5. **Delete User**

![Deleteuser](https://github.com/Van-Hoang-Kha/AWS-FCJ-Management/blob/master/images/deleteuser.png)

### How to usage
1. Git clone repository
```
https://github.com/Van-Hoang-Kha/AWS-FCJ-Management
```

2. Go to folder project
3. Dependencies Installation
4. Configuration Server
5. Restarting Express server
6. Start our local server

### Dependencies Installation
```
npm install express dotenv express-handlebars body-parser mysql
```
### Configuration Server
Create a .env file and add your database credentials like this:
```
DB_HOST = 'localhost'
DB_NAME = 'DB_NAME'
DB_USER = 'root'
DB_PASS = 'password'
```
### Restarting Express server
```
npm install --save-dev nodemon
```

### Start our local server

```
npm start
```

### SQL Schema

```
CREATE TABLE `lib'.`user` ( `id` INT NOT NULL AUTO_INCREMENT , `first_name` VARCHAR(45) NOT NULL , `last_name` VARCHAR(45) NOT NULL , `email` VARCHAR(45) NOT NULL , `phone` VARCHAR(45) NOT NULL , `comments` TEXT NOT NULL , `status` VARCHAR(10) NOT NULL DEFAULT 'active' , PRIMARY KEY (`id`)) ENGINE = InnoDB;
```
### SQL Dummy Data

```
INSERT INTO `user` 
(`id`, `first_name`,  `last_name`,    `email`,                 `phone`,         `comments`, `status`) VALUES
(NULL, 'Amanda',      'Nunes',        'anunes@ufc.com',        '012345 678910', '',          'active'),
(NULL, 'Alexander',   'Volkanovski',  'avolkanovski@ufc.com',  '012345 678910', '',          'active'),
(NULL, 'Khabib',      'Nurmagomedov', 'knurmagomedov@ufc.com', '012345 678910', '',          'active'),
(NULL, 'Kamaru',      'Usman',        'kusman@ufc.com',        '012345 678910', '',          'active'),
(NULL, 'Israel',      'Adesanya',     'iadesanya@ufc.com',     '012345 678910', '',          'active'),
(NULL, 'Henry',       'Cejudo',       'hcejudo@ufc.com',       '012345 678910', '',          'active'),
(NULL, 'Valentina',   'Shevchenko',   'vshevchenko@ufc.com',   '012345 678910', '',          'active'),
(NULL, 'Tyron',       'Woodley',      'twoodley@ufc.com',      '012345 678910', '',          'active'),
(NULL, 'Rose',        'Namajunas ',   'rnamajunas@ufc.com',    '012345 678910', '',          'active'),
(NULL, 'Tony',        'Ferguson ',    'tferguson@ufc.com',     '012345 678910', '',          'active'),
(NULL, 'Jorge',       'Masvidal ',    'jmasvidal@ufc.com',     '012345 678910', '',          'active'),
(NULL, 'Nate',        'Diaz ',        'ndiaz@ufc.com',         '012345 678910', '',          'active'),
(NULL, 'Conor',       'McGregor ',    'cmcGregor@ufc.com',     '012345 678910', '',          'active'),
(NULL, 'Cris',        'Cyborg ',      'ccyborg@ufc.com',       '012345 678910', '',          'active'),
(NULL, 'Tecia',       'Torres ',      'ttorres@ufc.com',       '012345 678910', '',          'active'),
(NULL, 'Ronda',       'Rousey ',      'rrousey@ufc.com',       '012345 678910', '',          'active'),
(NULL, 'Holly',       'Holm ',        'hholm@ufc.com',         '012345 678910', '',          'active'),
(NULL, 'Joanna',      'Jedrzejczyk ', 'jjedrzejczyk@ufc.com',  '012345 678910', '',          'active')
```

### Reference
[Nodejs Documents](https://nodejs.org/en/docs/)

[MySQL Documents](https://dev.mysql.com/doc/)

[Simple User Management System – Nodejs, Express, MySQL & Handlebars](https://raddy.dev/blog/simple-user-management-system-nodejs-express-mysql-handlebars/)


