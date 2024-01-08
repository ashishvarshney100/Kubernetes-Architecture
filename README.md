The main components of the Master/Control Plane Node:
====================================================

API Server: It exposes the Kubernetes API, handling requests and serving as the front-end for the Kubernetes control plane.

Kube Scheduler: It's responsible for scheduling pods to run on nodes, based on resource availability and other constraints.

Kube Controller Manager: Manages various controllers that regulate the state of the cluster, such as node controller and replication controller.

etcd: A distributed key-value store that stores the cluster's configuration data, ensuring consistency across the cluster.

Cloud Controller Manager: Interacts with the underlying cloud provider's API to manage resources such as load balancers or storage, but it's optional and depends on the cloud provider.

The main components of Worker/Data Plane Node:-
==============================================

Kubelet: It ensures that containers are running in a Pod and communicates with the master node.

Kube-proxy: It maintains network rules on nodes, enabling communication across Pods and services.

Container Runtime(Optional):- A container runtime is the software responsible for running containers. 
