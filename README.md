# phpinfo

```
git clone https://github.com/JoseMgil/phpinfo
cd phpinfo
git checkout main
```
```
php -f src/index.php -S 0.0.0.0:8080
```
```
curl localhost:8080/src/index.php
```

# Instruciones para construir la imagen docker
```
git checkout santander

docker build --file Dokerfile --tag manyogil/phpinfo:santander . 
```

