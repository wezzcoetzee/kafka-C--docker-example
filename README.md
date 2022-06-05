# kafka C# docker example

I wanted to make a quick example application for my own reference and this is what I typed into Google to find one. Much to my surprise there wasn't anything that was complete, so here we are!

## Prerequisites

- Docker
- IDE

## Commands

To get Kafka up and running just run `docker-compose up -d` from your terminal/commandline.

Create the topic from your terminal/commandline

```
docker compose exec broker \
  kafka-topics --create \
    --topic purchases \
    --bootstrap-server localhost:9092 \
    --replication-factor 1 \
    --partitions 1
```