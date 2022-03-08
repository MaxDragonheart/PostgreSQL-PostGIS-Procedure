# INSTALL PgAdmin4 on Ubuntu
Procedure tested on UBUNTU 20.04

You must have PostgreSQL already installed. Import the repository signing GPG key:
```
curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add -
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/focal pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list' 
```
Update your repositories:
```
sudo apt update
```
Install PgAdmin:
```
sudo apt install pgadmin4
```
Choice login data for PgAdmin4 web interface
