# postgres-CLI-command
---
## start, stop postgres server 

```shell
$ sudo service postgresql start
$ sudo service postgresql stop
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
