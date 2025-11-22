# k8s-pod

## Kubernetes Pod Deployment — Overview

This project demonstrates how to deploy a basic application inside a Kubernetes cluster using a Pod manifest (nginx-pod.yaml). A Pod is the smallest deployable unit in Kubernetes and represents a single instance of a running process in your cluster.

In this deployment, the Pod is configured to:

Run a container based on a specified image (e.g., Nginx, custom app image, etc.)

Expose the application internally so it can be accessed by other components in the cluster

Maintain a consistent environment using defined specifications such as container ports, resources, and restart policies

This setup is ideal for learning:

How Kubernetes manages containers

How Pods are defined using YAML

How to deploy and inspect workloads (kubectl apply, kubectl get pods, kubectl describe pod)

How applications run inside Kubernetes compared to running directly with Docker

This deployment will be a foundation for building more advanced Kubernetes objects such as Deployments, ReplicaSets, and Services.

## Pod Structure - For Reference

Pod (root)
├── metadata (branch)  
│   ├── name (leaf)  
│   └── labels (leaf)  
└── spec (branch)  
    └── containers (branch)  
        └── - name, image, ports (leaves)  