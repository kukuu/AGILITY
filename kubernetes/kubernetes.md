# Kubernetes

Kubernetes is a clustering architecture and provides all the orchestration and plumbering of nodes together. A typical configuration for a production environment could possibly have up to five machines. Normal recommendation is to have 3 (odd number to avert contention for resources if 1 fails) masters and 2 nodes for redundancy, resiliency and availability .

## Components

1. Pod 

Pods are wrappers, and provides abstraction for Kuubernetes on how to run  multiple containers to access CPU, Network resources to enable scaling. They are labelled to give  taxonomy to the pods. For referencing and managing. Pods interract with containers during run time.

Kubernetes uses Docker containers to deploy apps.

2. Controllers

Controllers manage Pods, and are packaged as replica sets to scale. They work on a set of rules

3. Jobs

Another use case of running pods is jobs. They can run as cron jobs (start, run and terminate). They can be invoked on triggers (as Cron jobs) or manually.

4. Services

This is a exposure of pods, replicca sets and controllers on a port through the Kube proxy.

## Tools 

1. Kubeadm 

This is an administration tool for setting up and managing Kubernetes clusters. This runs on the Kubernetes host

2. Kubectl

This is the command line interface for interracting with Kubernetes clusters

3. Minikube

A utility for setting up single node instances of Kubernetes for testing and development.