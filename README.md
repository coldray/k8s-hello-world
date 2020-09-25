# Hello world

## Getting started
Learn Fundamentals of Kubernetes Deployment in coursera

### Deploy to k8s

install kubectl
install minikube

```
minikube start
eval $(minikube docker-env)
docker build -t golang-hello:ver1.1 .
kubectl create deployment golang-hello --image golang-hello:ver1.1
kubectl get deployments
kubectl get pods
kubectl create service loadbalancer golang-hello --tcp=8500:8500
minikube service golang --url
```

### Common Issues

[I am getting errimagepull error](https://stackoverflow.com/questions/40600419/why-am-i-getting-an-errimagepull-error-in-this-kubernetes-deployment)
