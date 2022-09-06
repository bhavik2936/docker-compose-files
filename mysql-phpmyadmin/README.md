# MySQL-phpMyAdmin Docker Compose
It contains docker instances for both **MySQL** & **phpMyAdmin** internally connected via bridge network.

### MySQL
MySQL, the database server itself can be accessed on host machine (localhost) on port _3306_.

#### Description
Below configuration are already set by default via `mysqlCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 3306  | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |

### phpMyAdmin
phpMyAdmin is integrated to graphically visualize the mysql database.
It can be accessed on host machine (localhost) web browser at http://localhost:8080.

#### Configuration
Below configuration are already set by default via `phpmyadminCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 8080  | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |
