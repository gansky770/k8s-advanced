# k8s-advanced
INIT-LAB.

1.Created ConfigMap with the k/v source=https://...

2.1 Created a Pod with init container (image alpine/git:latest )

2.2 Created an EMPTYDIR volume and mount it as /cdn 

2.3 Inside the container there is COMMAND "git clone $SOURCE (the SOURCE is ENV from Configmap 

3 Created main Image(in the same pod kind) nginx:latest  mounte /usr/share/nginx/html to Emptydir

4 Created Service that expose the app on port 80 

5 Created an ingress Rule to direct traffic on port 80 to our SVC

Tested on Minikube with nginx ingress contoller and Loadbalancer imulator (minikube tunnel)

Thank you!
# k8s-advanced
INIT-LAB.

1.Created ConfigMap with the k/v source=https://...
2.1 Created a Pod with init container (image alpine/git:latest )
2.2 Created an EMPTYDIR volume and mount it as /cdn 
2.3 Inside the container there is COMMAND "git clone $SOURCE (the SOURCE is ENV from Configmap 
3 Created main Image(in the same pod kind) nginx:latest  mounte /usr/share/nginx/html to Emptydir
4 Created Service that expose the app on port 80 
5 Created an ingress Rule to direct traffic on port 80 to our SVC
Thank you!
