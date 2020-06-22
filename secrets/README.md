Create a secret:

  kubectl create secret generic <secret-name> --from-literal=<key>=<value> --from-literal=<key2>=<value2> ...

  kubectl create secret generic <secret-name> --from-file=<path-to-file> --from-file=<path-to-file2> ...

Get secret details:

  kubectl get secret <secret-name> -o yaml
