# Welcome to Bootcamp
## Docker 101 Guideline
### Docker Build
```
docker build  -t welcomebootcamp:0.0.1 .
docker image ls
docker run -p 80:80 welcomebootcamp:0.0.1
docker ps
docker stop [container id]
docker ps -a
docker exec -it [container id] sh
docker stop [container id]
```
### Docker Ship
```
docker login
docker tag welcomebootcamp:0.0.1 sal2apao/welcomebootcamp:0.0.1
docker push sal2apao/welcomebootcamp:0.0.1
```
### Docker Run
```
docker pull sal2apao/welcomebootcamp:0.0.1
docker run -d -p 80:80 sal2apao/welcomebootcamp:0.0.1
```

### Clean up
```
docker stop $(docker ps -a -q)
docker rm [container id] -f
docker rm $(docker ps -a -q)
docker rm $(docker ps -a -f status=exited -q)
docker rmi [image id]
docker rmi $(docker images -a -q)
docker system prune -a
```

### Reference Document
[Docker Cheat Sheet](https://www.docker.com/sites/default/files/d8/2019-09/docker-cheat-sheet.pdf)

[Dockerfile Cheat Sheet](https://kapeli.com/cheat_sheets/Dockerfile.docset/Contents/Resources/Documents/index)