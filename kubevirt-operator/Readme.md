# Kubevirt 

This folder contains the manifest to install the kubevirt operator.

## Update the operator for all clusters
To update the operator across deployments, change the url of the base in the kustomization.yaml file to point to the new version.

for example:

```yaml
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization

resources: 
- https://github.com/kubevirt/kubevirt/releases/download/v0.58.0/kubevirt-operator.yaml
```
installs the operator version 0.58.0

## Update the operator for a specific cluster
TBD