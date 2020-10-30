### Instructions
From within the \_create_helper execute the following to create the skeleton
for a new Helm chart, passing in the chart name
```
go run main.go <folder> <chart>
```

Once the core files have been added to the chart folder add values to the `values.yml` file.

### Dry run
```
helm install frontend-service-viewer ./frontend-service-viewer -f ../common-values.yml -f ./dev-common-values.yml -f ./dev-secrets.yml --dry-run
helm upgrade frontend-service-viewer ./frontend-service-viewer -f ../common-values.yml -f ./dev-common-values.yml -f ./dev-secrets.yml --dry-run
```
