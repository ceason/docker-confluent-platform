
### Running Confluent Platform
```
docker-compose up
```

-----


### "Direct container access" Setup

#### Add route to docker-machine
* Windows: `route -p add 172.25.0.0 mask 255.255.0.0 {{DOCKER_MACHINE_IP}}`
* OSX: `sudo route add 172.25.0.0/16 {{DOCKER_MACHINE_IP}}`

#### Put in /etc/hosts
```
172.25.1.101 confluent-zookeeper
172.25.1.102 confluent-kafka
172.25.1.103 confluent-schema-registry
172.25.1.104 confluent-kafka-connect
172.25.1.105 confluent-control-center
```

