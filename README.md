# openshift-cicd-demo
Openshift CI/CD provisioner demo

# Requirements

- Running OpenShift 3.9
- oc installed

# Steps
- CI/CD Stack warm up
- Deploy CI/CD Stack
- Deploy CI-Manager
- Initialise CI/CD Stack via CI-Manager
- Image Streams setup
- Setup deployment strategies per environment
- Deploy pipeline
- Start pipeline

- Start pipeline

## CI/CD Stack warm up
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-create-projects
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-admin-setup
```

## Deploy CI/CD Stack
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-deploy-stack
```

## Deploy CI-Manager
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-deploy-ci-manager
```

## Initialise CICD Stack via CI-Manager
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-ci-manager-initialiser
```

## Image Streams setup
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-image-streams-setup
```

## Setup deployment strategies per environment
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-deployment-strategies-setup
```

## Deploy pipeline
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-deploy-pipeline
```

## Start pipeline
```
OPENSHIFT_URL=https://myopenshift-console.me:8443 ./demo-cicd-start-pipeline
```
