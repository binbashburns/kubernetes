## About
Kubernetes is a platform for running containers. 

It takes care of starting your containerized applications, rolling out updates, maintaining service levels, scaling to meet demand, securing access, and much more. 

The two core concepts in Kubernetes are the **API**, which you use to define your applications, and the **cluster**, which runs your applications. 


A **cluster** is a set of individual servers that have all been configured with a container runtime like Docker, and then joined into a single logical unit with Kubernetes. The picture below shows a high-level view of the cluster.

![Container Orchestration](./img/1.jpeg)

The Kubernetes cluster is there to run your applications. You define your apps in *YAML* files and send those files to the Kubernetes API. Kubernetes looks at what you’re asking for in the YAML and compares it to what’s already running in the cluster. It makes any changes it needs to get to the desired state, which could be updating a configuration, removing containers, or creating new containers.

![Clusters and Containers](./img/2.jpeg)

Those YAML files are properly called application manifests, because they’re a list of all the components that go into shipping the app. Those components are Kubernetes resources; they have proper names, too. The picture below takes the concepts from other photos and applies the correct Kubernetes resource names.

![Kubernetes Objects](./img/3.jpeg)

