# WebBits

https://store.docker.com/images/mysql

docker run --name gv-web-bits-mysql -p 8080:8080 -e MYSQL_ROOT_PASSWORD=gv-web-bits -d mysql:latest

docker run --name gv-web-bits-wordpress --link gv-web-bits:mysql -p 8080:80 -d wordpress:latest
