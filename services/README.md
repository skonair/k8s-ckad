Create the yaml template for a CLusterIP service on port 6379 

  kubectl create service clusterip redis-service --tcp=6379 --dry-run=client -o yaml

  kubectl set selector service/httpd 'run=httpd'
