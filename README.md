# README

Config files for Holodrive's MatchMaker

## Setup
```
ssh root@<ip> -i <ssh-key>
curl https://bitcake.github.io/holodrive-matchmaker-config/docker-compose.yml -O
docker login
```

## Docker Compose
```
docker-compose up
docker-compose down
```

----

## Docker Stack
```
docker stack init
docker stack deploy -c docker-stack.yml holodrive-matchmaker
```

```
docker stack ls
docker stack ps holodrive-matchmaker
docker stack rm holodrive-matchmaker
```

## Other Docker Commands
```
docker pull bitcakestudio/holodrive-matchmaker:latest
docker run -d --network host --restart always --name matchmaker-a -e "APP_TAG=a" bitcakestudio/holodrive-matchmaker

docker ps
docker container ls -a
docker container logs -f --tail 50 matchmaker-a

docker kill
docker container prune -f
```
