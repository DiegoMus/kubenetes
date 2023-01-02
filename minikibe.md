tener permisos de sudo para el usuario de docker
poder utilizar los siguiente comandos:

minikube start --driver=docker -p clusterDEV --nodes=2
minikibe delete -p clusterDEV
minikuve profile nombrecluster


kubectl run nginx1 --image=nginx
kubectl get pods
kubectl get pods -o wid


kubectl exec nginx1 -- ls
kubectl exec nginx1 -it  -- bash
kubectl logs apache

kubectl expose nginx --name nginx-svc-md --port=80 --type=LoadBalancer
