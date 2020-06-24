User in case you need two services togehther (e.g. log agent and web server)

Multiple types:
- Ambassador
- Adapter
- Sidecar

But: the pod definition always looks the same

Sidecar:
e.g. a log container next to  a server. the log sidecar connects to the logging server

Adapter:
e.g. a log adapter changes the format of the container logs to a common one before sending it to a central server

Ambassador:
e.g. a log ambassador will proxy the requests to a log database based e.g. on the stage
