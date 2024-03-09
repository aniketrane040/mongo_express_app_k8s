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

---------------------------------

create ip for external service using minikube command :

-> minikube service mongo-express-service

output :
|-----------|-----------------------|-------------|---------------------------|
| NAMESPACE |         NAME          | TARGET PORT |            URL            |
|-----------|-----------------------|-------------|---------------------------|
| default   | mongo-express-service |        8081 | http://192.168.64.2:30000 |
|-----------|-----------------------|-------------|---------------------------|
🎉  Opening service default/mongo-express-service in default browser...

