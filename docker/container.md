
Docker operates on a client-server architecture. A client, in this docker-cli course, i.e. Docker's command line interface, comes to query a daemon, docker daemon using a REST API. It is this daemon that takes care of the various tasks of building and managing images, launching containers. Finally, a last important component of Docker are the Docker registries, which are image directories that the Docker daemon will query to download an image to launch. DockerHub was the public directory generally used by Docker users, but in some cases, in particular with the enterprise editions of Docker, trusted registries are used instead, that is to say private directories.

Finally, note that the exact operation of Docker and containers in general is managed by the Linux system of the host machine or by its emulator if you are working on a Windows machine.

Ubuntu
```
docker --version
```
Launch Docker daemon
```
sudo service docker start
```
Launch docker image
```
docker container run imagename
```

List docker images
```
docker image ls
```

Run a container with interaction
```
docker container run -it ubuntu:latest
```

List docker containers
```
docker container ls
```

To list also stopped containers
```
docker container ls --all
```

