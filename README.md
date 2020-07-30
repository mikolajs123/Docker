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
