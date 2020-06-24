Readiness Probes

Pod Status vs Pod Conditions

Pod status:
- Pending (Waiting for a node)
- ContainerCreating (image pulled)
- Running

Shown in 'kubectl get pods'

Pod Comnditions: 
Array of boolean values, e.g.
- PodScheduled
- Initialized
- ContainersReady
- Ready (application inside pod is ready and accept requests)

Shown in 'kubectl describe pod <pod-name>' and check 'Conditions:'


Readiness probes, e.g.
- http test
- tcp test
- exec command


Liveness probes
tests periodically if the application in a container is healthy

