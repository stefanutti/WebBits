# webbits

- docker run --name webbits-mysql -e MYSQL_ROOT_PASSWORD=webbits -p 14010:8080 -d mysql:latest
- docker run --name webbits-wordpress --link webbits-mysql:mysql -p 14020:80 -d wordpress:latest
