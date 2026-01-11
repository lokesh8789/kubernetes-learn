# Get Namespace
--> kubectl get namespace or kubectl get ns

# Create ns
--> kubectl create ns <ns_name> 

# Delete ns
--> kubectl delete ns <ns_name>

# Get pods running under specific ns
--> kubectl get pod -n <ns_name>

# Create resources under specific ns
--> kubectl apply/create -f <yaml_file> -n <ns_name>