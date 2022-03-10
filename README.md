# k8s-cluster-vagrant-ansible (courtesy @krystek17)

Configuration to set up a multi-node kubernetes cluster with the help of Vagrant and Ansible. It's meant to work with Ubuntu 20.04 and libvirt (instead of VirtualBox).

## To deploy and run nodes

vagrant up

## Cluster configuration

You can configure your k8s cluster by editing the CONFIGURATION VARIABLES available in the Vagrantfile.

## Kubectl configuration

kubectl config view

kubectl get nodes

## Connection to master node via ssh

vagrant ssh master
