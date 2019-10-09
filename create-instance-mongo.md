```sh
$ docker run --name my-container-mongo -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=123 -v ~/workspace/docker-volumes:/data/db -d  mongo:4.2.0-bionic
$ docker exec -it my-container sh
# mongo
> use admin
> db.auth('root','123')
> show databases
```
