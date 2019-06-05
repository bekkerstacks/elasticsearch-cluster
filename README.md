# elasticsearch-cluster
Elasticsearch Cluster on Docker Swarm


### Options

Other Versions:

```
image: docker.elastic.co/elasticsearch/elasticsearch-oss:${ELASTIC_VERSION:-6.7.0}
```

Healthchecks:

```
   healthcheck:
      test: ["CMD-SHELL", "curl --silent --fail localhost:9200/_cluster/health || exit 1"]
      interval: 30s
      timeout: 5s
      retries: 3
```
