convert docker compose file to kubernetes yaml
https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/#kompose-convert
```sh
cd /Users/joeqiao/Documents/LocalHub/kafka/kafka-connect/kubernetes
kompose -f ../docker-compose.yml  convert
```


move image from docker hub to acr
```sh
az acr import --name acraksnativeinteastus2deveastus2hptf --source docker.io/kong/kubernetes-ingress-controller:2.3.1 --image kong/kubernetes-ingress-controller:2.3.1
```
