convert docker compose file to kubernetes yaml
https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/#kompose-convert
```sh
cd /Users/joeqiao/Documents/LocalHub/kafka/kafka-connect/kubernetes
kompose -f ../docker-compose.yml  convert
```


move image from docker hub to acr
```sh
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/landoop/fast-data-dev:cp3.3.0 --image landoop/fast-data-dev:cp3.3.0
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/landoop/fast-data-dev:1.1.1 --image landoop/fast-data-dev:1.1.1
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/lensesio/fast-data-dev:2.3.0 --image lensesio/fast-data-dev:2.3.0
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/itzg/elasticsearch:2.4.3 --image itzg/elasticsearch:2.4.3
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/postgres:9.5-alpine --image joelearnkafka/postgres:9.5-alpine
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/postgres:14.4 --image joelearnkafka/postgres:14.4
```
