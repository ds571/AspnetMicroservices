# Docker Commands
```
// List all docker containers (running and stopped)
docker ps -aq

// Remove all containers
docker rm $(docker ps -aq)

// Remove all images
docker rmi $(docker images -q)

// Prune Images
docker system prune
```

# AspnetMicroservices
AspnetMicroservices

```
// Running MongoDb
docker run -d -p 27017:27017 --name shopping-mongo mongo

// Getting MongoDb Logs
docker logs -f shopping-mongo

// Shell access:
docker exec -it shopping-mongo bash

// Manual Mongo Commands:
mongo // enter mongo cmd
show dbs // show space used
use CatalogDb // switch to db
db.createCollection('Products') // Create collection
db.Products.remove({}) // Remove collection
show databases
show collections
```
