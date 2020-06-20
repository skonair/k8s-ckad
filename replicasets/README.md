Replication controller (older technology)
- scales pods up and down
- checks the 
- load balances the application

Replica Set (new technology and recommended)
- scales pods
- selector needs to be defined (replication controller assumes the template pods as default)


How to scale the replicas
- update in the definition file and run $ kubectl replace -f replicaset-definition.yaml
- kubectl scale -- replicas=6 -f replicaset-defintion.yaml
- kubectl scale -- replicas=6 replicaset myapp-replicaset


