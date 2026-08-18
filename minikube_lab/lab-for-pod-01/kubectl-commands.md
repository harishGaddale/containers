kubectl create -f nginx-pod-manifest-01.yaml --namespace lab

kubectl get pods -n lab

kubectl describe pod nginx-pod -n lab
