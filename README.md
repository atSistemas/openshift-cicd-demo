# openshift-cicd-demo
Openshift CI/CD provisioner demo

# Requirements

- Running OpenShift 3.9
- oc installed
- system user must have adm policy add-cluster-role-to-user cluster-admin enabled
- developer/any user must exist in order to run the demo

# Steps
- CI/CD Stack warm up
- Deploy CI/CD Stack
- Deploy CI-Manager
- Setup deployment strategies per environment
- Initialise CI/CD Stack via CI-Manager
- Start pipeline

## CI/CD Stack warm up
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-create-projects
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-admin-setup
```

## Deploy CI/CD Stack
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-deploy-stack
```

## Deploy CI-Manager
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-deploy-ci-manager
```

## Setup deployment strategies per environment
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-deployment-strategies-setup
```

## Initialise CICD Stack via CI-Manager
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-ci-manager-initialiser
```

## Start pipeline
```
OPENSHIFT_URL=https://change.this.openshift.url:8443 ./demo-cicd-start-pipeline
```

# Bootstrap

You can either run the demo following the previous steps o just run the bootstrap changing the OPENSHIFT_URL accordingly.

## Start pipeline
```
./boostrap
```