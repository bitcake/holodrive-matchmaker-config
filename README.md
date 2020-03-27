# README

Config files for Holodrive's MatchMaker

## Setup
```
ssh root@<ip> -i <ssh-key>
curl https://bitcake.github.io/holodrive-matchmaker-config/docker-compose.yml -O
docker login
docker-compose pull
```

## Docker Compose
```
docker-compose up
docker-compose top
docker-compose logs -f --tail 50
docker-compose down
```
