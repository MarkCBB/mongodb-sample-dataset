# [MongoDB Sample Dataset]

> this is a fork of [repo](https://github.com/mcampo2/mongodb-sample-databases).

> the original repo has BSON dump. I've removed it and I added a bash [script](https://github.com/neelabalan/mongodb-sample-dataset/blob/main/script.sh) to import the JSON to respective db 

## Running in docker

```bash
docker pull mvertes/alpine-mongo

docker run -d --name mongo -p 2717:27017 -v ~/mongodb:/data/db mvertes/alpine-mongo

# args
#   hostname   
#   port
./script.sh localhost 2717

# start mongo shell
docker exec -it mongo mongo
```
