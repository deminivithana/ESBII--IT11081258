####ESBII Lab 05 - Setting up Owncloud

# Install OwnCloud 7 on CentOS 7  #

**ownCloud** is a web suite that provides a cloud storage over the network, data can be uploaded via web browser or using software client. Data will be stored on the server and can be downloaded or access any time with browser or desktop client or smartphone app. 

## Prerequisites ##

1. It is based on PHP and database combination, database can be SQLite, MySQL, Oracle or PostgreSQL. So install PHP, Apache web server and MySQL server on CentOS 7. 

![](https://cloud.githubusercontent.com/assets/13186210/9331799/fc36b354-45de-11e5-8e1d-0b620ef74d9b.png)


2.Set SELinux to allow OwnCloud to write the data.

![](https://cloud.githubusercontent.com/assets/13186210/9331817/24dc9986-45df-11e5-85b4-b94ae1654e99.png)

3.Allow apache in firewall.

![](https://cloud.githubusercontent.com/assets/13186210/9331846/406ac010-45df-11e5-841f-3d22d57d233d.png)

4.Start Apache and MariaDB.

![](https://cloud.githubusercontent.com/assets/13186210/9331905/8419a72c-45df-11e5-8782-310ef569f26f.png)

5.Auto start the service at system start-up.

![](https://cloud.githubusercontent.com/assets/13186210/9331944/c116783a-45df-11e5-9bed-8b1722a2fb0b.png)



## Download and Setup ##

1.Download ownCloud from official website or enter the fallowing command on terminal and extract the archive.

![](https://cloud.githubusercontent.com/assets/13186210/9331984/1ec0c1ca-45e0-11e5-9e5c-29533577c496.png)



2.Allow the web server to read and write the files on cloud directory.

![](https://cloud.githubusercontent.com/assets/13186210/9332043/5f36da6e-45e0-11e5-8b5a-3fd42651e841.png)



## Create Database ##

1.MariaDB server must be started before creating the database, login to MySQL server.

![](https://cloud.githubusercontent.com/assets/13186210/9332081/8ce62bb8-45e0-11e5-96cc-e58ccf8db8b8.png)

2.Create database called “clouddb”. Allow “clouddbuser” to access the “clouddb” database on localhost with predefined password.

![](https://cloud.githubusercontent.com/assets/13186210/9332098/ad1fe70c-45e0-11e5-8607-6bf36d9450d6.png)




## Configure Apache server ##

While configuring Apache web server, it is recommended that you to enable .htaccess to get a enhanced security features, by default .htaccess is disabled in Apache server.

1.To enable it, open your virtual host file and make AllowOverride is set to All.

![](https://cloud.githubusercontent.com/assets/13186210/9332147/e9eb7d04-45e0-11e5-8f90-75d35b39e160.png)


2.Restart all services related to Apache server.

![](https://cloud.githubusercontent.com/assets/13186210/9332213/327f2980-45e1-11e5-8784-89b78cbb7644.png)

## Configure ownCloud  ##

Open up web browser, point a URL to http://127.0.0.1/owncloud.
It must be configured before going to live. Enter admin user name, password


![](https://cloud.githubusercontent.com/assets/13186210/9332230/4bf12da0-45e1-11e5-834c-be1722b96ee4.png)

![](https://cloud.githubusercontent.com/assets/13186210/9332241/57c782fa-45e1-11e5-8af5-ab91f8ad72c5.png)

![](https://cloud.githubusercontent.com/assets/13186210/9332251/64a6b1ee-45e1-11e5-9d68-01cdb0c9a774.png)

![](https://cloud.githubusercontent.com/assets/13186210/9332263/6d76e8b6-45e1-11e5-8c76-e547d686ba84.png)
