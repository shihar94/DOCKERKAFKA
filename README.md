# DOCKERKAFKA
Docker Compose for starting kafka and zookeeper in local host. Through this a multi container can be managed in docker for running kafka and zookeeper. This minimizes the need to run all the kafka bash files as usual process. 

Prerequisite 
    Docker Compose (This will be installed when docker is installed)

To Start services Execute Following Command
```sh
docker-compose up -d 
```

Executing following command to check if the services are up and running
``` sh 

docker ps            
CONTAINER ID   IMAGE                       COMMAND                  CREATED         STATUS                            PORTS                                        NAMES
bdbe1cd03321   confluentinc/cp-kafka       "/etc/confluent/dock…"   9 seconds ago   Up 7 seconds (health: starting)   0.0.0.0:9092->9092/tcp                       kafka
395efb17e683   confluentinc/cp-zookeeper   "/etc/confluent/dock…"   9 seconds ago   Up 7 seconds (health: starting)   2888/tcp, 0.0.0.0:2181->2181/tcp, 3888/tcp   zookeeper
```


To Stop Services Execute the following command
```sh
docker-compose stop 
```


