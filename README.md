# Docker
run new container with named 'webhost' in background nginx
```bash
docker container run --publish 80:80 --detach --name webhost nginx
```
stop container
```bash
docker container stop webhost
```
stop container
```bash
docker container stop webhost
```
docker container rm -f 247
docker container ls == docker ps
docker container ls -a == docker ps -a
docker container rm 247 bcd 420 # remove only first three letters
docker container top webhost
logs webhost
docker container logs webhost
docker version
docker info
docker container run -d -p 3306:3306 --name db -e MYSQL_RANDOM_ROOT_PASSWORD=yes mysql
docker container run -d --name webserver -p 8080:80 httpd
docker container run -d --name proxy -p 80:80 nginx
curl localhost
curl localhost:8080
docker container top db # processes in certain container
docker inspect db -> details container config in json
docker container stats # get live view of all containers like top in linux
docker container run -it --name proxy nginx bash # create container and terminal inside of it
exit # exit bash from terminal
docker container run -it -name ubuntu ubuntu
docker container start -ai ubuntu
docker container port webhost # show all busy port on container
docker network ls -> show networks
docker network inspect -> inspect network
docker network inspect -> inspect network
docker network create ${name} -> inspect network
docker network connect ${network} ${container} -> connect network to container
docker network disconnect ${network} ${container} -> disconnect network to container
docker container run -d --name new_nginx --network my_app_net nginx
docker container run -rm -it ubuntu:14.04 bash 
docker pull nginx
docker pull nginx:1.11.9
