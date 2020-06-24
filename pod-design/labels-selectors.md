Labels
- properties attached to an object


e.g. Pods:
...
   metadata:
     labels:
       app: App
       function: front-end
       

Selectors
- help you filter objects

  kubectl get pods --selector app=App1
  kubectl get pods --selector bu=finance,tier=frontend,env=prod


Annotations
- provide additional information

...
metadata:
  name: simple-webapp
  labels:
    app: app1
    function: front-end
  annotations:
    buildversion: 1.34
spec:
  ...
