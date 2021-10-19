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

docker build --file Dockerfile --tag manyogil/phpinfo:santander . 
```

# Instruciones para construir la imagen docker optimizada
```
git pull

docker build --file Dockerfile_optimizado --tag manyogil/phpinfo:santander-optimizado . 

docker push manyogil/phpinfo:santander-optimizado
```

