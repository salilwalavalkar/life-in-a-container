### Docker commands

#### Build
docker-compose build

docker-compose up -d

#### To remove all containers:
docker rm $(docker ps -a -q)

#### To remove all images:
docker rmi $(docker images -q)

#### List images
docker images

#### Remove an image
docker rmi <image-id>

#### Container shell access
docker exec -it <container-name> bash

#### List ports
docker port <container-name>

#### List processes
To see the processes running in a container, you can use the top command (similar to running the Linux top command):

docker top <container-name>

#### View container log file
docker logs <container-name>

#### Follow container log file
docker logs --follow <container-name>

or

docker logs -f <container-name>

#### Restart a running container
docker restart

#### Stop all running containers
docker stop $(docker ps -a -q)

#### Inspect container information
docker inspect <container-name-or-id>
