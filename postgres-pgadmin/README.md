# Postgres-pgAdmin Docker Compose
It contains docker instances for both **PostgreSQL** & **pgAdmin** internally connected via bridge network.

### PostgreSQL
Postgres, the database server itself can be accessed on host machine (localhost) on port _5432_.

#### Description
Below configuration are already set by default via `pgCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 5432  | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |

### pgAdmin
pgAdmin is integrated to graphically visualize the postgres database.
It can be accessed on host machine (localhost) web browser at http://localhost:8088.

#### Configuration
Below configuration are already set by default via `pgAdminCreds.env` file and can be modified by overriding the same.

| Config   | Value              | Comment                                                           |
| -------- | ------------------ | ----------------------------------------------------------------- |
| Port     | 8088               | Exposed at localhost (127.0.0.1)                                  |
| Username | admin@postgres.com |                                                                   |
| Password | pgadmin            |                                                                   |
| Host     | postgres           | To connect docker instance server of postgres database in pgAdmin |
