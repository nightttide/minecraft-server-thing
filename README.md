# minecraft-server-thing

```bash
sudo apt-get update

#latest java runtime from microsoft on ubuntu 22.04 (2023-10-12)
```
curl -sSL -O https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
rm packages-microsoft-prod.deb
sudo apt-get install msopenjdk-21

mkdir minecraft_server
cd minecraft_server

#latest server (2023-10-12)
wget https://piston-data.mojang.com/v1/objects/5b868151bd02b41319f54c8d4061b8cae84e665c/server.jar

echo "eula=true" > eula.txt

echo "java -Xmx1024M -Xms1024M -jar server.jar nogui" > start.sh
chmod +x start.sh

./start.sh
```
