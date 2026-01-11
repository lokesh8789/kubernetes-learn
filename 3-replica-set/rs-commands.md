# Get Replica Set
--> kubectl get replicaset or kubectl get rs

# Create rs
--> kubectl create -f <rs_yaml_file>

# Delete rs
--> kubectl delete -f <rs_yaml_file>

# More Details about rs
--> kubectl describe rs

# More Details about individual rs
--> kubectl describe rs <rs_name>