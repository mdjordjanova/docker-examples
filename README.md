### List contanier images

```bash
docker image ls
```

### List running containers

```bash
docker container ls
docker container ls --all
```


### Remove unused docker images

```bash
docker image prune
docker image prune --all
docker image remove {id}
```

### Remove unused docker containers

```bash
docker container prune
```

### Kill docker container

```bash
docker container kill {id}
```

### Build docker container
```bash
docker build .
docker build -t $name .
```

### Open shell in a docker container
```bash
docker exec -it $container bash
```

### Volume redirect to local machine
```bash
docker run --rm --detach                                \
                --volume "$PWD/logs":/var/log/ping-log  \
                test
```

### Run docker container and remove after exit

```bash
 docker run --rm
```

### 
```bash
docker run -t --rm --name=test test:0.0.1 
docker stop test
```

### Ubuntu shell:
```
docker run -t -i --rm --name=test ubuntu /bin/bash
```

### Examples starting Ubuntu docker container
```bash
docker run ubuntu
docker run ubuntu bash
docker run --interactive --tty ubuntu #docker run -it ubuntu
```

### Reources
- [DockerHub](https://hub.docker.com/search?q=&type=image)
- [Multi-Stage Build](https://docs.docker.com/develop/develop-images/multistage-build/)
- [Alpine](https://hub.docker.com/_/alpine)