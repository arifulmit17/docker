docker run -d --restart unless-stopped --name unless-test alpine sleep 1d

docker inspect -f '{{.RestartCount}}' restart-always

docker run -it --name restart-always --restart always alpine

docker run -it --name test-container ubuntu bash

docker container rm d2c3

docker stop d9f

<!-- video 55.5  commands-->

docker volume create my-volume

docker volume ls

docker volume rm my-volume

docker run -it --name test-container -v my-vol:/data ubuntu bash

docker volume prune

<!-- video 55.8  commands-->

docker build --build-arg APP_ENV=testing -t my_app .

docker run -it --rm -p 5000:5000 my_app:latest