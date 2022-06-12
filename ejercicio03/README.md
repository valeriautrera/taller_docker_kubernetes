Para ver las layers de cada imagen se usaron los comandos:
```shell
docker inspect nicopaez/passwordapi-java:java8-alpine | jq .[].RootFS.Layers
docker inspect nicopaez/passwordapi-java:java8-fabric | jq .[].RootFS.Layers
```

La imagen `nicopaez/passwordapi-java:java8-alpine` tiene 4 layers

La imagen `nicopaez/passwordapi-java:java8-fabric` tiene 9 layers

Para ver si tienen layers en común se corrió el comando:
```shell
comm -1 -2  --nocheck-order  <(docker inspect nicopaez/passwordapi-java:java8-alpine | jq .[].RootFS.Layers) <(docker inspect nicopaez/passwordapi-java:java8-fabric | jq .[].RootFS.Layers)
```

Tienen en común la primer layer:
"sha256:73046094a9b835e443af1a9d736fcfc11a994107500e474d0abf399499ed280c",



