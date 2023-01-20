
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
that returns:  
```
    ubuntu@ip-172-31-40-119:~$ docker container run hello-world                                                                                                             Hello from Docker!
    This message shows that your installation appears to be working correctly. To generate this message, Docker took the following steps:
    1. The Docker client contacted the Docker daemon.
    2. The Docker daemon pulled the "hello-world" image from the Docker Hub.(amd64)
    3. The Docker daemon created a new container from that image which runs the executable that produces the output you are currently reading.
    4. The Docker daemon streamed that output to the Docker client, which sent it to your terminal.
    To try something more ambitious, you can run an Ubuntu container with:
    $ docker run -it ubuntu bash 
    Share images, automate workflows, and more with a free Docker ID:                                                                                   ```  
https://hub.docker.com/   
    For more examples and ideas, visit:                                                                                                                   https://docs.docker.com/get-started/
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

When you create a Docker image, you give it a name that makes it easy to identify. You can also give it a tag or a label that allows you to differentiate between different versions of the same image. If no tag is specified, Docker considers that the tag used is latest. For the same name, or the same repository, we can have several different tags that coexist. In addition, a unique id is assigned to it when the image is downloaded or created locally: the id corresponds to the hashed image.
