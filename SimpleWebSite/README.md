## Build docker Створюємо image
```
docker build -t spr311-docker .

docker images --all

docker login

docker tag spr311-docker:latest novakvova/spr311-docker:1.0

docker push novakvova/spr311-docker:1.0
```

## Working server up docker images
```
docker images
docker pull novakvova/spr311-docker:1.0
docker ps -a
docker run -d --restart=always --name spr311_container -p 4728:8080 novakvova/spr311-docker:1.0

docker ps -a

```