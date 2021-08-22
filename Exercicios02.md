
### Question 1
Get the Pods from all namespaces.

Write down its content.

### Question 2
Create a namespace called ns-5.

Create a Pod named nginx with the image nginx:1.17.4.

Expose the container on port 80.

Write down the list of Endpoints for the current namespace.

### Question 3
Create a Pod named busybox with the image busybox:1.31.0.

From within the Pod busybox, retrieve the path / on the Pod nginx.

Write down its content.

### Question 4
Create a Service named entrypoint that targets the Pod nginx on port 80.

The Service should be of type NodePort.

Write down the YAML file for the entrypoint Service.

### Question 5
Create a Deployment named haproxy.

The Deployment should:

uses the haproxy:2.0.7 image
exposes port 80
have 3 replicas
Expose the Deployment with a Service of type ClusterIP named ingress.

From within the Pod busybox, retrieve the path / on the Service ingress.

Write down its content.

### Question 6
Write a Service of type ClusterIP that target Pods from the Deployment haproxy and the Pod nginx.

Write down the list of Endpoint for that Service.