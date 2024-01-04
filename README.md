# Unifi Network Application
https://hub.docker.com/r/linuxserver/unifi-network-application

These files will allow the Linuxserver.io Unif Network Application to run on Raspberry Pi 4 with Mongodb 4.4.18.

Edit the docker-compose.yml as needed for your installation such as ports. If you require access from outside your local network poke holes in your router's firewall as needed.

```
mkdir -p $HOME/docker/unifi-network-application
```
```
cd $HOME/docker/unifi-network-application
```
```
wget https://github.com/slochewie/docker-compose-files/raw/main/unifi-controller/docker-compose.yml
```
```
docker-compose pull
```
```
docker-compose up -d
```

First launch of UniFi Controller will take some time for it to initialize, but eventually go to https://ip-of-your-pi:8443 to begin setup of the controller.



## Author

Aaron Wilson <https://niteowl.dev>

[![](https://cdn.buymeacoffee.com/buttons/default-blue.png)](https://www.buymeacoffee.com/slochewie)

## License

[MIT License](./LICENSE)