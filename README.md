docker run --name mysql -e MYSQL_ROOT_PASSWORD=Password1234 -d mysql


docker run --name wordpress --link mysql -p 8185:80 -e WORDPRESS_DB_HOST=mysql:3306 -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=Password1234 -e WORDPRESS_DB_NAME=wordpress -e WORDPRESS_TABLE_PREFIX=wp_ -d wordpress

Docker

Introduction
Benefits of Docker
Images vs Containers
Container vs VM
The underlying technology
Installation of Docker engine and client
Running container as BG and Non-BG
Hello world example
linking containers
List containers
Passing environment variables
Investigating containers and images
Dockerfile and Registries
Dockerfile introduction
Dockerfile commands
Building Dockerfile
Creating Images
Type of registries
Pull/Push to specific registry
Storage and data persistence
