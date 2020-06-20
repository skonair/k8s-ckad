Ways to create a k8s pod:
- create a yaml file and apply that
- kubectl run <podname> --image=<image>

Display additional information about pods, like node

  kubectl get pods -o wide

Under READY there are the number of running containers/total containers displayed.

Update a pod info:
- edit the given pod definintion file or
- kubectl get pod <pod-name> -o yaml > pod-definition.yaml (edit file, delete and re-create the pod)
- kubectl edit pod <podname> (to edit pod properties)

