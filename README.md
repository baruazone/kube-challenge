# kube-challenge

This repository holds some kubernetes resource definitions. Deploying those creates an environment with backend `redis` component that requires to be observed and dealt with.

## System Requirements

This will run on any kubernetes environment. Either of the below approaches can be followed to set up a local one.

* Install docker desktop Or
    * [Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/)
    * [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/install/)
    * Enable Kubernetes

* [Install Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)

## Steps to create the objects

* Clone the repo
* Run `kubectl apply -f development.yaml`
* Run `kubectl apply -f redis-master-deployment.yaml -n development`
* Run `kubectl apply -f frontend-service.yaml -n development`
* Observe what's happening to the resources (e.g. Running accordingly?)
* Detect and resolve if there's any issue

## Outcomes

* Write a brief report 
* Send it back to HR or
* Bring it over during the interview