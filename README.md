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
```

### Examples starting Ubuntu docker container
```bash
docker run ubuntu
docker run ubuntu bash
docker run --interactive --tty ubuntu #docker run -it ubuntu
```

### Reources
- [DockerHub](https://hub.docker.com/search?q=&type=image)