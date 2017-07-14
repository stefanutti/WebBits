# webbits

- docker run --name gv-webbits-mysql -e MYSQL_ROOT_PASSWORD=gv-webbits -p 14010:8080 -d mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 14020:80 -d wordpress:latest
