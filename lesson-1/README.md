# docker-lesson-1
Docker lesson-1 content

![docker](https://user-images.githubusercontent.com/47666526/105575118-30242300-5d7a-11eb-91aa-9d195e33ffc1.png)


```
sudo usermod -aG docker $USER
```

```
docker run busybox echo "Hello world"
```

```
docker ps
```

```
docker ps -a 
```

```
docker images
```

```
docker images -a 
```

```
docker build -t kuber .
```

```
docker run -p 8080:8000 -d kuber:latest
```

```
docker logs put_here_docker_id -f
```

```
docker exec -it put_here_docker_id /bin/bash
```

```
docker commit put_here_docker_id kuber:0.1
```

```
docker tag kuber:0.1 bokovets/kuber:0.1
```

```
docker tag kuber:latest bokovets/kuber:latest
```

```
docker login
```

```
docker push bokovets/kuber:0.1
```

```
docker push bokovets/kuber:latest
```

```
docker stop put_here_docker_id
```

```
docker rm put_here_docker_id
```

```
docker rmi kuber:0.1 
```

```
docker rm -vf $(docker ps -a -q)
```

```
docker rmi -f $(docker images -a -q) 
```