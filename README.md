# CodingWithKubernetes

How to code a web app composed of two web service :
- a frontend
- a backend

# Prerequisite

This tutorial assume that you have already installed Kubernetes. If not, follow this other tutorial: https://github.com/charroux/kubernetes

# The backend app

The backend is coded in Java (Spring boot), but it doesn't matter. The Web service simply return "World :" when it receives an HTTP Get on "/hello": https://github.com/charroux/CodingWithKubernetes/blob/master/BackEnd/src/main/java/com/example/BackEnd/MyWebService.java

# The frontend app

The frontend (also coded in Java Spring boot request the backend service and concataines the result "World !" with "Hello": https://github.com/charroux/CodingWithKubernetes/blob/master/FrontEnd/src/main/java/com/example/FrontEnd/FrontEndApplication.java

# Kubernestes configuration file

A single yaml file is enough to configure the cluster: https://github.com/charroux/CodingWithKubernetes/blob/master/front-back-app.yml

It contains :

## The backend deployment


