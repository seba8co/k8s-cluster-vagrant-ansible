# k8s-cluster-vagrant-ansible

Configuration to set up and deploy a multi-node kubernetes cluster with the help of Vagrant and Ansible. It's meant to work with Ubuntu 20.04 and libvirt (instead of VirtualBox).

## Nodes deployment

vagrant up --provider=libvirt

## Cluster configuration

You can configure your k8s cluster by editing the CONFIGURATION VARIABLES available in the Vagrantfile.

## Kubectl configuration

kubectl config view

-Test your config like the example bellow :

kubectl get nodes

-Result:

```
NAME     STATUS   ROLES                  AGE   VERSION
master   Ready    control-plane,master   11m   v1.23.4
node-2   Ready    <none>                 10m   v1.23.4
```

## Connection to nodes via ssh

-Master access:

vagrant ssh node-1

-Worker access:

vagrant ssh node-2

Courtesy [krystek17](https://github.com/krystek17)
