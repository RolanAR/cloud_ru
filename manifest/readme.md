Kubernetes

minikube start

kubectl create namespace rolanspace

kubectl apply -f deployment.yaml

проверка работоспособности

kubectl get pods -n rolanspace -o wide

kubectl port-forward svc/your-app-service -n rolanspace 8000:80

проверка Readiness и Liveness пробы

kubectl logs NAME POD -n rolanspace
