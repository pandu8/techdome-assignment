# techdome-assignment

**STEP1: clone the repos which are given to us**
Here is the repos :
Backend: https://github.com/Anand-1432/Techdome-backend
Frontend: https://github.com/Anand-1432/Techdome-frontend

**STEP2: Creating Dockerfiles for Frontend and Backend services**
>>cd into frontend folder and create Dockerfile for frontend
>>cd into fbackend folder and create Dockerfile for bacend

**STEP3: Setup docker-compose file** 
>>write docker compose file for all 3 services and its dependencies in root directory of project (docker-compose.yaml)
>>build the compose file with below command. it will create images and run containers of all 3 services
    docker-compose up -d

****STEP4: Kubernetes setup** 
>>write deployment files for all 3 services in root directory of project
1. frontend-deployment.yaml
2. backend-deployment.yaml
3. db-deployment.yaml

>>Now start minikube --> minikube start

**STEP5: Applying Kubernetes Manifets (use below commands to apply)**
kubectl apply -f frontend-deployment.yaml
kubectl apply -f backend-deployment.yaml
kubectl apply -f db-deployment.yaml

**check the pods and services**
>>kubectl get po
>>kubectl get svc

>>Finally Access our application using
http://localhost:3000

