Kubernetes cluster is made up of master(control-plane) and nodes.

# Components of Master Node(Control-Plane):-
1. api-server -> apis for client to talk to the cluster
2. etcd -> distributed key value store to store cluster data
3. controller-manager -> A process which continuosly monitors workloads/nodes etc.
4. scheduler -> workload scheduler

# Components of Worker Node:-
1. kubelet -> an agent which creates containers and monitors them
2. container runtime(docker) -> to create container, we need to have container runtime in the node
3. kube-proxy -> maintains the network rules on the node for communication among workloads in the cluster


# Check for kubectl version details:
--> kubectl version --output=yaml or kubectl version --output=json

# kubectl client checks for server details from te path:
--> cat ~/.kube/config