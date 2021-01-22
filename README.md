# airflow

## commands
```
kubectl create deployment airflow --image=puckel/docker-airflow:latest --dry-run -o yaml > airflow_deployment.yml
kubectl expose deployment airflow --type=NodePort --port=8080 --dry-run -o yaml > airflow_service.yml
kubectl apply -f airflow_deployment.yml
kubectl apply -f airflow_service.yml
```


