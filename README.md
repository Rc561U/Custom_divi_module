# Wordpress-Docker-compose template.


### 1.Instalation:
```shell
docker-compose up
```
```shell
sudo chmod 777 app/
```

```shell
bash install.sh
```


### Add to wp-config.php
```
define('FS_METHOD', 'direct');
```
### Create DIVI extension
```shell
cd wp-content/plugins/
npx create-divi-extension my-extension
cd my-extension
yarn start
```