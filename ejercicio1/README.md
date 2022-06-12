Instrucciones:

Buildear imagen:
```shell
docker build -t vutrera-nginx .
```

Correr contenedor:
```shell
docker run --name vutrera-ej1-nginx -d -p 8080:80 vutrera-nginx
```

Acceder a la url:
http://localhost:8080
