# Kubernetes
Learning kubernetes

Pod- pod is smallest unit in kubernetes which is collection of one or more containers
Kubernetes Architecture:
In kubernetes we have 2 planes:
1. control plane[master node]
2. data plane[worker node]
control plane components are:
Api server: which is used to accept the request and decide on which node the pod has to get created.
scheduler: used to acts upon the information received from api server to scheduler the resources.
etcd: is key-value pair used to store the cluster information
controller manager: in kubernetes we have many controllers like replica controller. the controller manager is used to manage all the controllers to be up and running.
cloud controller manager[ccm]: this is specially used only for cloud deployments not for on-premises. If we need kubernetes to be created on new cloud then we have to write some logic and submit it to CCM.
data plane componenets are:
kubelet: creating pod and responsible to ensure pod is up and running else it has to take action.
kube-proxy: provides networking [like assigning ip address] and load-balancing
container runtime: used to run the container in pod.

