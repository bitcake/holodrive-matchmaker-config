# README

Config files for Holodrive's MatchMaker

## Deploy
```
ssh root@<ip> -i <ssh-key>
curl https://bitcake.github.io/holodrive-matchmaker-config/docker-stack.yml -O
docker stack init
docker stack deploy -c docker-stack.yml holodrive-matchmaker
```

## Manage
```
docker stack ls
docker stack ps holodrive-matchmaker
docker stack rm holodrive-matchmaker
```
