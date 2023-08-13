### k8s

### Services
* port types
  -> Port => service port
  -> TargetPort => pod's container port 
  -> NodePort => port exposed in Node
* Types
  * Nodeport
    -> port is opened in all the nodes in the cluster
    -> works anywhere anytime
    -> port range **30000 - 32767**
    -> Not a ideal way but useful in dev testing
  * LoadBalancer
  * External IP
  * Ingress     
