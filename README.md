# Linux Server Configuration
This project helped me to set and secure a Linux server instance and hosted Catalog App running live on a secure web server.

## IP address and SSH Port
IP address of the server: **18.234.230.53**
SSH Port of the server: **2200**

## Complete URL to the Catalog Application
URL of the application: **http://18.234.230.53.xip.io/**

## Softwares Installed
Installed softwares: **apache2**, **libapache2-mod-wsgi**, **python-dev**, **python-pip**, **python-flask**, **python-sqlalchemy**, **python-psycopg2**, **postgresql**

```bash
sudo apt-get install apache2 libapache2-mod-wsgi python-dev
```
```bash
sudo apt-get python-pip python-flask python-sqlalchemy python-psycopg2
```
```bash
sudo apt-get postgresql
```

Installed libraries: **oauth2client**, **requests**, **httplib2**

```bash
sudo pip install oauth2client requests httplib2
```

## Configuration done
1.  Changed the SSH port from **22** to **2200**. 
2.  Configured the Uncomplicated Firewall (UFW) to only allow incoming connections for **SSH (Port 2200)**, **HTTP (Port 80)**, and **NTP (Port 123)**.
3.  Configured the local timezone to UTC.
4.  Configured Apache to serve a Python mod_wsgi application (Catalog App)
5.  Configured PostgreSQL, by creating new database user **catalog** and a database named **catalog**, giving limited permissions and not allowing not remote connections.
6.  Used Full-Stack Web Developer: Deploying to Linux Server videos to setup the server and to get AWS Lightsail instance running.
