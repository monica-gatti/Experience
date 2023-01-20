
Docker operates on a client-server architecture. A client, in this docker-cli course, i.e. Docker's command line interface, comes to query a daemon, docker daemon using a REST API. It is this daemon that takes care of the various tasks of building and managing images, launching containers.

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

