# Innovation Lab Bootcamp
## Docker 101
## Guideline
```
docker build  -t welcomebootcamp:0.0.1 .
docker images
docker run -d -p 80:80 welcomebootcamp:0.0.1
docker stop [containerid]
docker ps
docker ps -a
docker exec -it [containerid] sh
```