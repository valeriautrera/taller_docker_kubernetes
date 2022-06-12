Instrucciones:

Desde la carpeta `ejercicio1` correr el comando:
```shell
docker run --name vutrera-ej1-nginx -v $PWD/html:/usr/share/nginx/html:ro -d -p 8080:80 nginx
```

Acceder a la url:
http://localhost:8080
