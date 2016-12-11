# php-dockerized-composed
Dockerized PHP development stack: Nginx, MySQL, PHP-FPM, Memcached

# Usage
```
cp .env.template .env
export ENV_FILE=".env"
docker-compose up
```

# Todo
Uppdatera image till att kopiera in alla filer



# Configuration
```
WWW_ROOT=./app/www

# PHP environment variables
PHP_CONFIG_FILE=./app/conf/php/php.ini

# NGINX environment variables
NGINX_DOCKER_IMAGE_VENDOR=nginx
NGINX_DOCKER_IMAGE_TAG=latest
NGINX_CONFIG_FILE=./app/conf/nginx/nginx.conf
NGINX_VHOST_ROOT=./app/conf/nginx/vhost
NGINX_LOG_ROOT=./app/logs/nginx
NGINX_HOST_PORT=80

# MYSQL environment variables
MYSQL_DOCKER_IMAGE_VENDOR=mysql
MYSQL_DOCKER_IMAGE_TAG=latest
MYSQL_USER=dev
MYSQL_PASSWORD=secret
MYSQL_ROOT_PASSWORD=secret
MYSQL_DATABASE=database
MYSQL_HOST_PORT=3306

# MEMCACHED environment variables
MEMCACHED_DOCKER_IMAGE_VENDOR=memcached
MEMCACHED_DOCKER_IMAGE_TAG=latest
MEMCACHED_HOST_PORT=11211

# XDEBUG environment variables
XDEBUG_CONFIG_FILE=./app/conf/xdebug/xdebug.ini

# BUILD options
INSTALL_XDEBUG=false
INSTALL_MCRYPT=false
INSTALL_PDO_MYSQL=false
INSTALL_PDO_PGSQL=false
```
