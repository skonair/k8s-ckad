Logging

View logs via

  kubectl logs -f <pod-name>

If multiple container run in a pod, one must specify the container.

  kubectl logs -f <pod-name> <container-name>



