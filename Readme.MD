docker run -d --restart unless-stopped --name unless-test alpine sleep 1d

docker inspect -f '{{.RestartCount}}' restart-always

docker run -it --name restart-always --restart always alpine

docker run -it --name test-container ubuntu bash

docker container rm d2c3

<!-- video 55.5  commands-->

docker volume create my-volume

docker volume ls

docker volume rm my-volume

docker run -it --name test-container -v my-vol:/data ubuntu bash

docker volume prune