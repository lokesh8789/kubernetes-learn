# Create deployment
--> kubectl create -f <deployment_yaml_file>

# Delete deployment
--> kubectl delete -f <deployment_yaml_file>

# More Details about deployment
--> kubectl describe deploy or  kubectl describe deployment

# Get deployment
--> kubectl get deployment or kubectl get deploy

# Create/Update deployment
--> kubectl apply -f <deployment_yaml_file>

# Get History of rollout deploy
--> kubectl rollout history deploy <deploy_name>

# rollback to previous version
--> kubectl rollout undo deploy <deploy_name>

# rollback to specific version
--> kubectl rollout undo deploy <deploy_name> --to-revision=<revision_number_found_using_rollout_history>

# Get Details of specific rollout deploy
--> kubectl rollout history deploy <deploy_name> --revision=<revision_number_found_using_rollout_history>

# Deployment Strategy
1. recreate
2. rolling update

- rolling update can be done using two properties:
    1. maxSurge -> max number/percentage of additional pods that can be created
    2. maxUnavailable -> max number/percentage of pods that can be terminated

