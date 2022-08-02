# Mongo Application

![Architecture-Flow](./images/architecture-flow.png "Architecture-Flow")

## To run this application using this configuration yaml file please follow below step.

1. Start minikube
```
minikube start
```
![Start minikube](./images/step-1-minikube-start.png "Start minikube")

2. Enable ingress addon using minikube
```
minikube addons enable ingress
```
![Enable ingress addon using minikube](./images/step-2-minikube-addons-ingress.png "Enable ingress addon using minikube")

3. Create "app-mongo" namespace in your cluster
```
kubectl create namespace app-mongo
```
![Create app-mongo namespace in your cluster](./images/step-3-namespace-app-mongo.png "Create app-mongo namespace in your cluster")

4. Launch configuration for mongo application
```
kubectl apply -f app-mongo-init.yml
```
![Launch configuration for mongo application](./images/step-4-launch-mongoexpress.png "Launch configuration for mongo application")

5. Verify mongo application
```
kubectl get all -n app-mongo; kubectl get ingress -n app-mongo
```
![Verify mongo application](./images/step-5-verify-mongoexpress.png "Verify mongo application")


## Takeaway points
* This application is handeling:
  1. Single domain and single path routing for ingress; You can configure it based on your requirement w.r.t. multidomain or multiple path type routing by updating ingress file.
  2. Protocol "http" only; You can configure it based on your requirement w.r.t. secure protocol by creating secret for the tls(ssl) and attaching it in ingress.
