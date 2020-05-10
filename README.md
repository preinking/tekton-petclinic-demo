# Caching Maven Dependencies in Tekton Pipelines

This is an example to show how to use workspaces in Tekton Pipelines for caching Maven dependencies and reducing build time by avoiding to download dependencies on every pipeline run.

```
kubectl create -f buildah.yaml
kubectl create -f git-clone.yaml
kubectl create -f kaniko.yaml
kubectl create -f maven.yaml
kubectl create -f resources.yaml
kubectl create -f secrets.yaml
kubectl create -f maven-pipeline.yaml
kubectl create -f maven-pipelinerun.yaml
```
