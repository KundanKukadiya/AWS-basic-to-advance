# ECS

Why Orchestrators
1. Manage lifecycle of containers create/restart/destroy
2. Deploy & load-balance application across multiple servers
3. Autoscalling to handle variance in traffic
4. Rolling out changes to application

### ECS launch types
1. EC2
2. Fargate - serverless

- ECS manages the containers
- Full control over your infrastructure

### EC2 vs Fargate
1. EC2
   - Manage to EC2 instance
2. Fargate
   - Follows a serverless architecture
   - Fargate wll create servers on demand
   - no need to provision/maintain EC2 servers
   - You only pay for what you use
     
### ECS Task Defination
> Blueprint of our containers

### ECS Service
> A service ensures that a certain number of tasks are running at all times
> Restarts containers that have exited/crashed
> Ec2 instace fails the service will restart task on a working EC2 instaces

### Load balancer
> A Load balancer can be assigned to route external traffic to your service

