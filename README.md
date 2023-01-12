# day2-bitnami-sealed-secret

This repository has the manifests to deploying Bitnami Sealed Secret and and configuring it to allow resources manage from ArgoCD

## Getting start

This project has been configured with Kustomize, so to apply the manifests just simply execute the following commands:

```
oc apply -k overlays/$ENV
```

Where $ENV is the environment where you need deploy on. Notice that you might need to add changes in order to satisfies your cluster environment requirements, so that your must apply that changes on overlays environment folders instead in base manifests.