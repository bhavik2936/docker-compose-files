# Mongo-Mongo-Express Docker Compose

It contains docker instances for both **Mongo** & **Mongo Express** internally connected via bridge network.

## Mongo

Mongo, the database server itself can be accessed on host machine (localhost) on port _27017_.

### Description

Below configuration are already set by default via `mongoCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 27017 | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |

An example of connection string to interact with MongoDB is as below.

[mongodb://root:root@localhost:27017](mongodb://root:root@localhost:27017)

## Mongo Express

Mongo Express is integrated to graphically visualize the mongo database.
It can be accessed on host machine (localhost) web browser at [http://localhost:8081](http://localhost:8081).

### Configuration

Below configuration are already set by default via `mongoExpressCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 8081  | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |
| BasicAuth Username | root | This will be used to authenticate the user when they open the express in the browser. |
| BasicAuth Password | root | This will be used to authenticate the user when they open the express in the browser. |

