# [Application from kodecloud voting app](https://github.com/kodekloudhub/example-voting-app-kubernetes)


## Helpful commands
```sh
kubectl create -f applications/voting-app/postgres-deploy.yaml
```
```sh
kubectl create -f applications/voting-app/redis-deploy.yaml
```
```sh
kubectl create -f applications/voting-app/result-app-deploy.yaml
```
```sh
kubectl create -f applications/voting-app/voting-app-deploy.yaml
```
```sh
kubectl create -f applications/voting-app/worker-deploy.yaml
```
```sh
kubectl get deploy
```
```sh
kubectl create -f applications/voting-app/postgres-service.yaml
```
```sh
kubectl create -f applications/voting-app/redis-service.yaml
```
```sh
kubectl create -f applications/voting-app/postgres-service.yaml
```
```sh
kubectl create -f applications/voting-app/result-app-service.yaml
```
```sh
kubectl create -f applications/voting-app/voting-app-service.yaml
```
```sh
kubectl get svc
```

## Accesible from below links
1. [localhost:30004/](http://localhost:30004/)
2. [localhost:30005/](http://localhost:30005/)
