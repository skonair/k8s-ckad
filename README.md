List all resources

  kubectl get all

Use -o wide for additional details

Use -o json for json output

USe -o name to only the resource name

Use --dry-run=client to test your command

  kubectl create namespace test-ns --dry-run=client -o yaml                                                [±master ✓]

apiVersion: v1
kind: Namespace
metadata:
  creationTimestamp: null
  name: test-ns
spec: {}
status: {}

Use -o yaml to output the resource definition

