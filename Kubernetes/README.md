# Kubernetes (K8)

Kubernetes is an open source system for managing and deploying containerised application.

### Benefits of using K8

**Automated Deployment and Scaling**

Kubernetes helps make sure your containers are doing their jobs and that you have the right number of them working at any given time. It does this by looking at all the computers available and managing the workers for you.

**High Availability**

When you deploy applications using Kubernetes, it distributes the workload across nodes (vm/servers). So, if you have a bunch of containers that need to run, Kubernetes will decide which nodes they should run on. This helps to balance the load and ensure that no single node gets overloaded.

If one node goes down or has a problem, the other nodes in the cluster can continue running the applications, helping to maintain high availability and prevent downtime.

**Easy Deployment and Updates**

Kubernetes makes it easy to set up and update programs. You just tell it what you want, and it takes care of the rest. If things change, it adjusts automatically. 


**Portable across cloud providers**

Kubernetes can run on different cloud platforms, like Amazon Web Services (AWS), Google Cloud, Microsoft Azure, and others.

### Why would you not use Kubernetes?

**Highly Static Workloads**: If your workloads don't change much over time and you don't need auto-scaling or automated deployment features, a simpler solution might be suitable.

**Lack of Containerised Workloads**:
If your applications are not containerised, then Kubernetes may not provide significant benefits.

## Kubernetes Deployment 

Kubernetes Deployment is a resource object in Kubernetes that manages a set of identical pods or replicas. 

