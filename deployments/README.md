descriptor file very similar to the replicaset one

To display all k8s resources

  kubectl get all 

Create a deployment desciptor

  kubectl create deployment webapp --image=kodekloud/webapp-color --dry-run=client -o yaml
