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

docker kill matchmaker-a
docker container prune -f
```
