user account (human) vs srvice account (machines)

Create a service account

  kubectl create serviceaccount <sa-name>

This create a serviceaccount and a token for that. The token is then stored in a secret.
The secret is then linked to the service account.

'default' serviceaccount is automatically mounted under /var/run/secrets/kubernetes.io/serviceaccount in a pod

