# Wordpress-Docker-compose template for development Divi modules.

## Setup: 
 1. **PHP 8.1**
2. **Nginx**
3. **Mariadb**
4. **Phpmyadmin** 
5. **Docker & Docker-compose**


### 1. Instalation:
```shell
docker-compose up
```
```shell
sudo chmod 777 app/
```

```shell
bash install.sh
```


### 2. Add to wp-config.php
```
define('FS_METHOD', 'direct');
```
### 3. Install the Divi theme manually (zip archive in root directory)
### 4. Dive into docker container
```shell
docker-compose exec php bash
```
### 5. Create Divi extension
```shell
cd wp-content/plugins/
npx create-divi-extension my-extension
cd my-extension
yarn start
```