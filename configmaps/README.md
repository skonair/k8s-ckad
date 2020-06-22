config maps store data in key-value-pairs

Two steps:
- create config map
- inject into pod

kubectl create configmap <config-name> --from-literal=<key>=<value> --from-literal=<key2>=<value2> ...

kubectl create configmap <config-name> --from-file=<path-to-file>


