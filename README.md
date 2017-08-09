# webbits

- docker run --name gv-webbits-mysql -e MYSQL_ROOT_PASSWORD=gv -p 14010:8080 -d mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 14020:80 -d wordpress:latest

- docker commit gv-webbits-mysql stefanutti/gv-webbits-mysql:1.0
- docker commit gv-webbits-wordpress stefanutti/gv-webbits-wordpress:1.0

- docker run --name gv-webbits-mysql -e MYSQL_ROOT_PASSWORD=gv -p 14010:8080 -d stefanutti/gv-webbits-mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 14020:80 -d stefanutti/gv-webbits-wordpress:latest

How it works:

- https://shibulijack.wordpress.com/2012/03/18/create-custom-forms-in-wordpress (forms + php callback)
