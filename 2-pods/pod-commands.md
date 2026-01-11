# Get Pods
--> kubectl get pod

# Get individual Pod
--> kubectl get pod <pod_name>

# Watch Pods handling
--> watch -t -x kubectl get pod

# Create Pod
--> kubectl create -f <pod_yaml_file>   (e.g-> kubectl create -f first-pod.yaml)

# Delete Pod
--> kubectl delete -f <pod_yaml_file>

# Delete individual pod
--> kubectl delete pod <pod_name>

# More Details about pod
--> kubectl describe pod

# More Details about individual pod
--> kubectl describe pod <pod_name>

# Update Existing Running Pod
--> kubectl apply -f <pod_yaml_file>

# Get pods along with labels
--> kubectl get pod --show-labels

# Get pods using labels filter
--> kubectl get pod -l dept=dept-1,team=team-1

# More info about pod
--> kubectl get pod -o wide

# More info about individual pod
--> kubectl get pod <pod_name> -o yaml

# Port Forwarding to talk to pod
--> kubectl port-forward <pod_name> <host-port>:<container-port>

# Check logs of pod
--> kubectl logs <pod_name>

# Check logs of specific container from pod
--> kubectl logs <pod_name> -c <container_name>

# Access To running pod
--> kubectl exec -it <pod_name> -- <command>   (e.g-> kubectl exec -it pod-1 -- bash)

# Access To running specific container from pod
--> kubectl exec -it <pod_name> -c <container_name> -- <command>   (e.g-> kubectl exec -it pod-1 -c nginx-1 -- bash)