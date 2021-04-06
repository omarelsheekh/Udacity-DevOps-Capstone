# Udacity-DevOps-Capstone
### The final project in the Udacity AWS DevOps course
### in this project we will make a CI/CD pipeline to deploy a simple web app
## steps
1. linting dockerfile
2. build the docker image
3. pushing the image to docker hub
4. create an AWS infrastructure using cloudformation if not existanse
5. configure infra using ansible
## configure infra
### if infra wasn't created before running the pipeline
1. install docker on host
2. install a simple k8s cluster (minikube)
3. install kubectl, helm & ingress
### finally
1. install the helm chart
2. update the ingress to point to the new service
## Configure CircleCI before running this pipeline
- context: AWS 
    - AWS_ACCESS_KEY_ID
    - AWS_DEFAULT_REGION
    - AWS_SECRET_ACCESS_KEY
- context: DOCKERHUB
    - DOCKERHUB_USERNAME
    - DOCKERHUB_PASSWORD