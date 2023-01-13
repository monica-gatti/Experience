## Docker build

- Launch Docker Desktop 
- Create the docker compose file ( file with extension yml)
- From Power Shell launch
```
PS C:\SourceCode\PyAndDocDb\docker> docker build -t docker-mongodb.yml .
```

## See active container
See active containers: please note that it's necessary -a to check all the container that drains disk space
```
docker ps -a
```

## Release disk space
To release disk space on Ubuntu.
1. Stop the container(s) using the following command:
```
docker-compose down
```
2. Delete all containers using the following command:
```
docker rm -f $(docker ps -a -q)
```
3. Delete all volumes using the following command:
```
docker volume rm $(docker volume ls -q)
```
After that, you can restart the containers using the following command:
```
docker-compose up -d
```
The same command didn't work on windows10. I had to use Troubleshoot --> purge in Docker Desktop inferface
