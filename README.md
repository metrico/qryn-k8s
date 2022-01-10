<img src='https://user-images.githubusercontent.com/1423657/147935343-598c7dfd-1412-4bad-9ac6-636994810443.png' style="margin-left:-10px" width=220>

# cloki-k8s
cLoki on Kubernetes Example


#### Requirements
You need to have a Kubernetes cluster, and the kubectl command-line tool must be configured to communicate with your cluster. It is recommended to run this tutorial on a cluster with at least two nodes that are not acting as control plane hosts. 

- Clickhouse K8s Cluster
- Configure access details in `cloki-deployment.yaml`

### Usage

```
kubectl apply -f cloki-service.yaml,cloki-deployment.yaml
```

Access your application

If you're already using minikube for your development process:
```
minikube service cloki
```

Otherwise, let's look up what IP your service is using!
```
kubectl describe svc cloki
```
