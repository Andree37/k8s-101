# Commands for kubectl and minikube

Kubectl is to access any Kubernetes components

## Minikube
- Start with: `minikube start --vm-driver=hyperkit`
- Stauts with: `minikube status`

## Kubectl
- Get node status: `kubectl get [nodes,deployment,pod,replicaset,...]`
- Create components `kubectl create [component]`
 - Create deployment: `kubectl create deployment NAME --image=image`
- Verify pod changes: `kubectl describe pod [pod name]`
- Debug pods: `kubectl logs [pod-name]`
- Get inside the terminal of container: `kubectl exec -it [pod name] -- bin/bash`
- Apply configuration file: `kubectl apply -f config-file.yaml`
- Delete configuration from file: `kubectl delete -f config-file.yaml`