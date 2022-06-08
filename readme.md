
```
cd myapplication-spring

mvn compile package

docker build -f src/main/docker/Dockerfile -t docker.io/burrsutter/myapplication-spring:1.0.0 .

docker login

docker push docker.io/burrsutter/myapplication-spring:1.0.0

```


```
cd myapplication-quarkus

mvn compile package

docker build -f src/main/docker/Dockerfile -t docker.io/burrsutter/myapplication-quarkus:1.0.0 .

docker login

docker push docker.io/burrsutter/myapplication-quarkus:1.0.0

```

```
kubectl apply -f myapplication-deployment-live-ready.yml
```