# INSTALL PostgreSQL on Ubuntu
Use PostgreSQL and PostGIS from command line. Tested on Ubuntu 20.04

## Install PostgreSQL
```
sudo apt update
sudo apt install postgresql
```
### Verifying
```
sudo su - postgres
psql
postgres-# \conninfo
postgres-# \q
```
### Creation of TestDB [OPTIONAL]
```
sudo -i -u postgres
psql
CREATE DATABASE testdb;
CREATE USER testuser;
ALTER ROLE testuser WITH CREATEDB;
ALTER USER testuser WITH ENCRYPTED PASSWORD 'test1234';
