# nginx deploy
kubectl create configmap defaultconf  --from-file=default.conf -n web
kubectl create -f nginx.pvc.yaml
kubectl create -f nginx.deploy.yaml
