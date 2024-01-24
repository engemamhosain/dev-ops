# dev-ops
# Command for kafka start

cd kafka && docker-compose -f kafka-compose.yml up -d
docker network create mynetwork
docker network connect mynetwork kafka
docker network connect mynetwork zookeeper