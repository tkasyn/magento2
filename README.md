# magento2
In this project, we are using:

Operating system: Ubuntu 16.04

Web Server: Apache2

Database Server: Mysql-server-5.7

PHP version: PHP-7.1


To begin we have to install docker and docker-compose on Ubuntu 16.04 server.

Then follow the steps:

1) Clone or download this repository as

git clone https://github.com/tkasyn/magento2.git

2) Set mysql root credentials and name of the database to be created . 
Go to ~/magento2/docker-compose.yml and change mysql root password in database_server in:
mysql_password=
mysql_database=

3) Download Magento 2 version up to 2.2.5 to dockerize and upload it in directory magento2 in parallel to docker-compose.yml.

Go to https://magento.com/tech-resources/download? .

4) Build the docker image using command

docker-compose build

5) Check the built image as:

docker images

6) Run the containers from built image as:

docker-compose up -d

7) Check the running docker containers by command:

docker-compose ps

docker ps

Now, our server setup is all ready, and we have to hit our domain name or IP to install Magento2. 
