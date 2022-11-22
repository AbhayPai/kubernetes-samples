# [Kubernetes Deployment Documentation](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#creating-a-deployment)

## Helpful commands
```sh
kubectl create -f path/yaml-file.yaml
```
```sh
kubectl get deployment
```
```sh
kubectl describe deployment deployment-name
```
```sh
kubectl edit deployment deployment-name --record
```
```sh
kubectl apply -f path/yaml-file.yaml --record
```
```sh
kubectl rollout status deployment/deployment-name
```
```sh
kubectl rollout history deployment/deployment-name
```
```sh
kubectl rollout undo deployment/deployment-name
```
