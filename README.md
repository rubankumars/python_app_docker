docker run --name mysql -e MYSQL_ROOT_PASSWORD=Password1234 -d mysql


docker run --name wordpress --link mysql -p 8185:80 -e WORDPRESS_DB_HOST=mysql:3306 -e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=Password1234 -e WORDPRESS_DB_NAME=wordpress -e WORDPRESS_TABLE_PREFIX=wp_ -d wordpress

