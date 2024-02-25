## EKS Cluster create steps

### Create cluster - 
- Type : EC2 Instace
  ```
  eksctl create cluster --name kundan-cluster --region us-east-2 --version 1.28 --node-type t2.micro --nodes-min 2 --nodes-max 3
  ```
- Type : Fargate
  ```
  eksctl create cluster --name kundan-cluster --region us-east-2 --version 1.28 --fargate
  ```
  
### Delete Cluster
```
kubectl get svc --all-namespaces
```
```
kubectl delete svc service-name
```
```
eksctl delete cluster --name prod
```
