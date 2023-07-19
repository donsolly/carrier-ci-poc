# My Java Microservice

This repository contains a Java microservice, a Jenkinsfile for building, testing, and deploying the microservice, and a Helm chart for deploying the microservice to a Kubernetes cluster.

## Prerequisites

- Java
- Jenkins
- Helm
- Kubernetes

## Build, Test, and Deploy with Jenkins

The Jenkinsfile defines a pipeline with stages for building the application, running unit tests, and deploying to a staging environment. To execute the pipeline, use Jenkins to run the Jenkinsfile.

## Deployment with Helm

The `helm` directory contains a Helm chart for the microservice. It includes a `values.yaml` file that you can customize to change the replica count, container image and tag, and service port.

To deploy the application, navigate to the helm directory and run the following command:

```bash
helm install [RELEASE_NAME] .
