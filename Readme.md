
# Start it

```
boot2docker start
eval "$(boot2docker shellinit)"
```


# Debug
## Log into a Docker container
docker exec -it <container-name> /bin/bash

## Test MQTT connection
```
mosquitto_pub -h 192.168.4.3 -u admin -P admin -t "bcx.xdk.test" -m "test"
```

## Deploy
Helpful commands:
```
brew install ssh-copy-id
ssh-copy-id ...
docker-machine create -d generic --generic-ip-address=192.168.1.200 plc

```
