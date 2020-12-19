# PostgreSQL-PostGIS
Use PostgreSQL and PostGIS from command line. Tested on Ubuntu 20.04

##Install PostgreSQL

$ sudo apt update
$ sudo apt install postgresql 


###Verifying

$ sudo su - postgres
$ psql
$ postgres-# \conninfo
$ postgres-# \q


###Creation of TestDB [OPTIONAL]

$ sudo -i -u postgres
$ psql
$ CREATE DATABASE testdb;
$ CREATE USER testuser;
$ ALTER ROLE testuser WITH CREATEDB;
$ ALTER USER testuser WITH ENCRYPTED PASSWORD 'test1234';

## Install PostGIS

$ sudo apt update
$ sudo apt install postgis


##Create PostGIS extensions (from here: https://postgis.net/install/ )

CREATE EXTENSION postgis;                       --> Enable PostGIS (includes raster)


###Additional exstensions [OPTIONAL]
If necessary, based on your project

CREATE EXTENSION postgis_topology;              --> Enable Topology
CREATE EXTENSION postgis_sfcgal;                --> Enable PostGIS Advanced 3D and other geoprocessing algorithms sfcgal not available with all distributions
CREATE EXTENSION fuzzystrmatch;                 --> fuzzy matching needed for Tiger
CREATE EXTENSION address_standardizer;          --> rule based standardizer
CREATE EXTENSION address_standardizer_data_us;  --> example rule data set
CREATE EXTENSION postgis_tiger_geocoder;        --> Enable US Tiger Geocoder


