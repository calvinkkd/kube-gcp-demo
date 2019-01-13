commands

Creating containers from docker repo

Create repo locally and upload to GitHub / git lab

git https://github.com/janakiramm/hellowhale.git

git clone https://github.com/janakiramm/hellowhale.git

Cd hellowhale

docker build . -t hellowhale

docker images

docker run -d -p8080 --name hellowhale hellowhale

Check  by url localhost:8080

docker login -u janakiramm -p DemoPassword@123

docker push janakiramm/hellowhale

Execute in kubernetes cluster

kubectl create deployment hellowhale --image janakiramm/hellowhale

kubectl get deployments

kubectl get pods

kubectl

kubectl expose deployment/hellowhale --port=8080 --name=hellowhalesvc --type=LoadBalancer

kubectl get svc

kubectl exec -it --user=root jenkins-1-6f88f74b78-rqtlc  bash


getting logged in  pod kubectl exec jenkins-1-6f88f74b78-rqtlc  -it /bin/sh

# hellowhale
Simple Docker Demo App




