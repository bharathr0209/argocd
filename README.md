# Architecture

<img src="ArgoCDOpenshift.jpg" width="1328"/>

## Workflow:

* Argo CD is a declarative, GitOps continuous delivery tool designed for Kubernetes

* OpenShift provides out-of-the-box support for ArgoCD with its' built-in GitOps Operator

* The development source code along side Infrastructure Helm charts are hosted on GitHub

* Build Artifacts based out of this source code is stored in DockerHub Artifact repository

* ArgoCD will continuously monitor the source repository hosted on GitHub

* When new changes are made to GitHub repository, ArgoCD will detect the changes and syncronizes the latest helm charts

* Deploys the new version changes to OpenShift managed by ROSA


# Prerequisites - Creation of Secret Manager Endpoint
* An active AWS Account
* Understanding of OpenShift
* Understanding of ArgoCD
* Existing ROSA cluster
* Existing GitHub Account
