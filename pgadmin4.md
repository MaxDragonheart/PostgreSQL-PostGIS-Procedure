# INSTALL PgAdmin4 on Ubuntu
Procedure tested on UBUNTU 20.04

You must have PostgreSQL already installed. Import the repository signing GPG key:
```
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list'
sudo curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add
```
Update your repositories:
```
sudo apt update && sudo apt upgrade
```
Install PgAdmin:
```
sudo apt install pgadmin4
```
Choice login data for PgAdmin4 web interface
