# poc-ai-deployment

Download chart dependencies:
```shell
helm dependencies build helm
```

Deploy airflow:
```shell
helm upgrade --install --namespace abb --create-namespace lblod-ai-poc helm