Instrucciones:

1. Pull de imagen a copiar:
```shell
docker pull nicopaez/pingapp:3.0.0
```

2. Copiar imagen en local:
```shell
docker tag nicopaez/pingapp:3.0.0 valeriautrera/taller-ej2:1.0.0
```

3. Login a dockerhub:
```shell
docker login
```

4. Push de la nueva imagen:
```shell
docker push valeriautrera/taller-ej2:1.0.0
```

Para descargarse la imagen:
```shell
docker pull valeriautrera/taller-ej2:1.0.0
```
