### Question 1
Get the Pods from all namespaces.

Write down its content.

### Question 2
Create a namespace called ns-2.

Create the following Pods in that namespace:

A pod called nginx1 with a single container running the nginx:1.7.9 image
A pod called nginx2 that has one container running the nginx:1.17.4 image
A pod called haproxy that has one container running the haproxy:2.0.7 image
All pods should have a label of type app=proxy.

Write down the output of kubectl get pods for the ns-2 namespace.

### Question 3
Retrieve all labels for the running container in the ns-2 namespace.

Write down its content.

### Question 4
Add additional labels to the Pods:

nginx1 should have a label of type webserver=nginx and a label of type version=1
nginx2 should have a label of type webserver=nginx and a label of type version=2
haproxy should have a label of type webserver=haproxy and a label of type version=1
Write down the output of kubectl get pods for the ns-2 namespace.

### Question 5
Annotate the Pods with the following annotations:

nginx1 should have an annotation of description="first deployment"
nginx2 should have an annotation of description="second deployment"

### Question 6
With a single command, retrieve the Pods with the label webserver=nginx.

Write down the command.

### Question 7
With a single command, retrieve the Pods with the label version=1.

Write down the command.

### Question 8
Retrieve the annotation for the haproxy Pod.

Write down its content.

### Question 9
Create a Deployment with the image nginx:1.17.4.

The Deployment should:

be called nginx
have 2 replicas
expose port 80
include the label webserver=nginx for all Pods
Write down the output of kubectl get pods and kuebctl get deployments for the ns-2 namespace.

### Question 10
Write down the YAML file for the ReplicaSet that was created by the nginx Deployment.

### Question 11
Downgrade the nginx Deployment to use the nginx:1.16.1 image.

Write down the output of kubectl get replicaset for the ns-2 namespace.

### Question 12
Downgrade, again, the nginx Deployment to use the nginx:1.7.0 image.

Write down the status of the rollout.

### Question 13
Inspect the history of the nginx Deployment.

Rollback to version 1.

Write down the output of history command for the nginx Deployment in the ns-2 namespace.

### Question 14
Scale the nginx Deployment to three replicas.

Write down the list of pods with label webserver=nginx.


