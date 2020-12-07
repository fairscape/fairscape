# Fairscape monorepo

This repo contains all code for all fairscape framework components and clients.

# FAIRSCAPE Installation Instructions

This tutorial will cover how to setup and install a **FAIRSCAPE** cluster and cover some of the basic API calls.  

# Requirements
 - Kubernetes Cluster ([HOW TO HERE](http://example.com/))
 - Kubectl installed and configured with cluster
 - FAIRSCAPE Kubernetes Manifest  ([Avaiable HERE](https://github.com/fairscape/deployment))

## Create all pods and services
Create all necessary pods with simple kubectl create command
```console
kubectl create -f fairscape.yaml 
```
## Create required database and buckets
Create stardog database and buckets in minio required by MDS and Transfer services. 
```console
kubectl exec stardog -- bash -c "/opt/stardog/bin/stardog-admin db create -o search.enabled=true -n ors"
kubectl exec minio  -- ash -c "mkdir -p data/breakfast"
```
## Test Services Functioning as Expected
Command below execs into pod within cluster and runs deployment tests to make sure all services are properly up and running. 
```console
kubectl exec testing-pod  -- bash -c "python3 deployment-tests.py"
```

If this completes with no errors your're all set!

Checkout the [FAIRSCAPE Demos] (https://github.com/fairscape/demo)) to learn more about uploading data and running jobs.
