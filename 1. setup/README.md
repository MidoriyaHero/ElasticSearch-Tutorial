# ElasticSearch Tutorial (on Ubuntu and Windows)

## Step 1: Setup ElasticSearch 
Go to this link
```
https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.15.0-windows-x86_64.zip
```
THen download the zip file and extract it.
If you are on Windows, follow this: 
```
https://www.elastic.co/guide/en/elasticsearch/reference/current/zip-windows.html#windows-enable-indices
```
If you are on Ubuntu, open terminal and run the following commands: 
```
cd /path-to-your-extract-elasticsearch/elasticsearch-8.15.0

./bin/elasticsearch
```
then ElasticSearch will start and give you a token.

copy the token to paste it in your kibana later.
## Step 2: Setup Kibana 
To install kibana, go to this link
```
https://www.elastic.co/downloads/kibana
```
Then download the zip file and extract it. Then run the following command in your terminal if you are on Ubuntu:

```
cd /path-to-your-extract-kibana/kibana-8.15.0

./bin/kibana
```

## Step 3:
After that, open your browser and go to http://localhost:5601/ (kibana) and paste the token you got from elasticsearch.

## That all you need to do to setup elasticsearch and kibana, let's go to the next one (add index, docs, search by dev tools on kibana).

## NOTE: TO handle the error: failed to determine the health of the cluster
GO to ./elasticsearch-8.15.0/config/elasticsearch.yml and change the following line:
```
xpack.security.enabled: true
```
to
```
xpack.security.enabled: false
```

