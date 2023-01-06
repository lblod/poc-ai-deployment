# poc-ai-deployment

## Deploy

Download chart dependencies:
```shell
helm dependencies build helm
```

Deploy airflow:
```shell
helm upgrade --install --namespace abb --create-namespace lblod-ai-poc helm
```

## Notes
The APIs are not exposed by default. There does exist a ClusterIP service per API.
You are expected to provide the necessary components for external access.