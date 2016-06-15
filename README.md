# docker-kibana

This is [Kibana 4.4.2](https://github.com/elastic/kibana) in a minimal 113MB Docker image. Images are tagged by Kibana versions.

## Running

```
docker run --name kibana \
           --detach \
           --publish 5601:5601 \
           -e KIBANA_ES_URL=<elasticsearch url> \
           bryanl/docker-kibana:latest
```

You could set `KIBANA_INDEX` env variable to set an index for Kibana's data.
