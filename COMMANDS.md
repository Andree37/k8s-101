# Commands for kubectl and minikube

Kubectl is to access any Kubernetes components

## Minikube
- Start with: `minikube start --vm-driver=hyperkit`
- Stauts with: `minikube status`
- Assign an external service with Minikube: `minikube service [external service name]`

## Kubectl
- Get node status: `kubectl get [nodes,deployment,pod,replicaset,...]`
- Create components `kubectl create [component]`
 - Create deployment: `kubectl create deployment NAME --image=image`
- Verify pod changes: `kubectl describe pod [pod name]`
- Debug pods: `kubectl logs [pod-name]`
- Get inside the terminal of container: `kubectl exec -it [pod name] -- bin/bash`
- Apply configuration file: `kubectl apply -f config-file.yaml`
- Delete configuration from file: `kubectl delete -f config-file.yaml`
- Describe endpoints of service `kubectl describe service [service name]`
- Deployed deployment configuration: `kubectl get deployment [deployment name] -o yaml > deployment-result.yaml`
- See namespaces: `kubectl get namespace`