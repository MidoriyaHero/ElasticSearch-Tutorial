# ElasticSearch Tutorial

## Step 1: Setup ElasticSearch
Create a docker-compose.yml file
```
volumes:
  esdata:
    driver_opts:
      device: ~/CODE/Elasticsearch/data
      o: bind
```
In this part you need to change the device's path to yours. 

Then run command on terminal:
```
docker-compose up
```