# postgres-CLI-command
---
## start, stop postgres server 

```shell
$ sudo service postgresql start
$ sudo service postgresql stop
```

## init folder to store data 

```shell
postgres@ac-all-series: $ /usr/lib/postgresql/10/bin/initdb -D /usr/local/pgsql/data
```

## Starting the Database Server
```
postgres@ac-all-series: $ /usr/lib/postgresql/10/bin/postgres -D /usr/local/pgsql/data
```
---
## start postgres 

```shell
$ sudo -u postgres psql
```

---

## start postgres with existing db

```shell
$ sudo -u postgres psql db_name
```

---

## set new password

```
postgres=# \password
```
---
## show all database
```
postgres=# \l
```
---
 
 ## connect to the database
 ```
 postgres=# \c database_name
 ```
 ---
##  show all tables in a database
```
postgres=# \dt
```
---
##  quit
```
postgres=# \q
```
---
