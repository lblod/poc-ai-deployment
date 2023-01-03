# poc-ai-deployment

Create a namespace:
```shell
kubectl create namespace abb
```

First create the nesessary persistent volume claims:
```shell
kubectl --namespace abb apply -f pvc-models.yaml
```

Deploy airflow:
```shell
helm upgrade --install airflow apache-airflow/airflow --namespace abb --values values.yaml
```