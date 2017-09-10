# webbits

## First run
- docker run --name gv-webbits-mysql -e MYSQL_ROOT_PASSWORD=gv -p 14010:8080 -d mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 14020:80 -d wordpress:latest

## Create a new image
- docker commit gv-webbits-mysql stefanutti/gv-webbits-mysql:1.0
- docker commit gv-webbits-wordpress stefanutti/gv-webbits-wordpress:1.0

## First run with the new image
- docker run --name gv-webbits-mysql -e MYSQL_ROOT_PASSWORD=gv -p 14010:8080 -d stefanutti/gv-webbits-mysql:latest
- docker run --name gv-webbits-wordpress --link gv-webbits-mysql:mysql -p 14020:80 -d stefanutti/gv-webbits-wordpress:latest

## Start/Stop
- docker start gv-webbits-mysql
- docker start gv-webbits-wordpress
- docker stop gv-webbits-wordpress
- docker stop gv-webbits-mysql

## Forms:
- Forms can be inserted manually inside a page or with one of the plugins of Wordpress, as for example:
  - http://ninjaforms.com/
  - http://www.gravityforms.com/

## PHP:
- If you want interact with php directly inside the page or post, you can try this plugin:
  - https://xyzscripts.com/

## Additional links:
- https://shibulijack.wordpress.com/2012/03/18/create-custom-forms-in-wordpress (forms + php callback)
