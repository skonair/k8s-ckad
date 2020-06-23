Taints and tolerations: What pods can be scheduled on a node

Taint go on a node (e.g. taint=blue)

  kubectl taint nodes <node-name> key=value:taint-effect

Remove a taint from a node:

  kubectl taint nodes <node-name> key=value:taint-effect-


taint-effects can be:
- NoSchedule
- PreferNoSchedule
- NoExecute

  e.g. kubectl taint nodes node1 app=blue:NoSchedule 


Toleration go on a pod 


