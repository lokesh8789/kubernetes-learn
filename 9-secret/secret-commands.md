# Create inline secret
--> kubectl create secret generic <secret_name> --from-literal=appUrl=abcd --from-literal=timeout=30

# Get Secret
--> kubectl get secret

# Get secret details
--> kubectl get secret -o yaml