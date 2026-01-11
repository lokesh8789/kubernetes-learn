# Create deployment
--> kubectl create -f <service_yaml_file>

# Delete deployment
--> kubectl delete -f <service_yaml_file>

# More Details about deployment
--> kubectl describe service or  kubectl describe svc

# Get deployment
--> kubectl get service or kubectl get svc

# Create/Update deployment
--> kubectl apply -f <service_yaml_file>

# Service Types

1. ClusterIP -> for communication within the cluster, cannot be accessed outside the cluster
2. NodePort -> open specific port in each node and using that can be accessed outside the cluster
3. LoadBalancer -> can be used to receive traffic outside the cluster but only in cloud providers (AWS/GCP etc.) 