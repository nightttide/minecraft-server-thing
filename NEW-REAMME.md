
```bash
sudo apt-get install docker
docker pull sirplexus/minecraft-server-standalone:latest

docker container create --publish 25565:25565/tcp --name "Crafty-Photonics" --env RAM=1G sirplexus/minecraft-server-standalone

docker container start Crafty-Photonics
```