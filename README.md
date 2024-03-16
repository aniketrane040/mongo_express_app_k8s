Requirements : 

1. minikube
2. kubectl
3. docker

---------------------------------
Deployment on k8s:

1. create secret : kubectl apply -f mongo-secret.yaml

2. create configmap : kubectl apply -f mongo-configmap.yaml

3. create mongodb deployment : kubectl apply -f mongo.yaml

4. create mongo-express deployment : kubectl apply -f mongo-express.yaml

5. create ingress : kubectl apply -f express-ingress.yaml

---------------------------------

create ip for external service using minikube command :

-> kubectl get ingress

map ingress ip with our hostname (mongo-express.com) in /etc/hosts to work locally
