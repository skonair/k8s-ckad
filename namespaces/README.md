There is always a 'default' namespace.

There is also kube-system (k8s internal) and kube-public (made available to all users).

Namespaces can have resource limits. They maintain a dns service.

Resource Quota in a namespace:

  apiVersion: v1
  kind: ResourceQuota
  metadata:
    name: compute-quota
    namespace: dev
  spec:
    hard:
      pods: "10"
      requests.cpu: "4"
      requests.memory: 5Gi
      limits.cpu: "10"
      limits.memory: 10Gi

Connection within the same namespace, simply refer to the pod-name.
To connect to another pod use <podname>.<namespace>.svc.cluster.local 

  kubectl create namespace dev-ns

  kubectl create -f pod-definition.yaml --namespace=dev (to create the pod in a specific namespace)

  or provide in the metadata: section of the definition file via namespace: dev

Change the namespace:

  kubectl config set-context $(kubectl config current-context) --namespace=dev

List all pods in all namespaces:

  kubectl get pods --all-namespaces
