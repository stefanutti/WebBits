# webbits

- docker run --name gv-webbits-mysql -p 8080:8080 -e MYSQL_ROOT_PASSWORD=gv-web-bits -d mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 9999:80 -d wordpress:latest
