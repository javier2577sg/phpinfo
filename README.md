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
# Intrucciones para clonar el repositorio
```
git clone https://github.com/JoseMgil/phpinfo
cd phpinfo
git checkout santander
```

# Instruciones para construir la imagen docker
```
docker build --file Dockerfile --tag manyogil/phpinfo:santander . 
```

# Instruciones para construir la imagen docker optimizada
```
git pull

docker build --file Dockerfile_optimizado --tag manyogil/phpinfo:santander-optimizado . 

docker push manyogil/phpinfo:santander-optimizado
```

# Instrucciones para ejecutar el contenedor 
```
docker run -d --entrypoint /usr/bin/php --name phpinfo -p 8080:8080 --restart always -v ${PWD}/src/index.php:/src/index.php:ro  manyogil/phpinfo:santander-optimizado -f src/index.php -S 0.0.0.0:8080
```


