Choose which node a pod is running on.

Define a node selector in a pod:
Before you can run a pod with a nodeSelector you have to label the node.

Label a node:

  kubectl label nodes <node-name> <label-key>=<label-value>

  kubectl label nodes node-1 size=Large

Limitations

  only one node selector is used
  one label, one node 

