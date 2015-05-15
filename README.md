## About:

This [Docker](http://www.docker.com/) image is built exactly as [digitalwonderland/docker-kibana](https://registry.hub.docker.com/u/digitalwonderland/kibana/), but is instead based on [java:7-jre](https://registry.hub.docker.com/u/digitalwonderland/base/), the very same as the official [elasticsearch](https://registry.hub.docker.com/_/elasticsearch/) and [logstash](https://registry.hub.docker.com/_/logstash/) images

## Additional Software:

* [Kibana](http://www.elasticsearch.org/overview/kibana/)

## Usage
Use with a linked container named `elasticsearch` and should be well. For instance:

    docker run --rm --name kibana -p 5601:5601 --link elasticsearch:elasticsearch bosr/kibana
