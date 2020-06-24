monitoring resource consumption

heapster vs Metrics server

1 metrics server per k8s cluster
- in memory solution

kubelet runs on every node
- receiving instr from master server
- running pods on the node
- cadvisor (retrieving perf metrics)

when metrics server is running:

  kubectl top node
  kubectl top pod
