To deploy Gitlab to k8s, first we deploy gitlab-operator using this command :
kubectl apply -n <namespace> -f gitlab-operator-kubernetes-1.0.0.yaml  
Wait for the Gitlab-operator change the status to success, then edit and deploy the Gitlab with the command below:
kubectl apply -n <namespace> -f gitlab.yaml
