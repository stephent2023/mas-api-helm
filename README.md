# api-helm-chart
This repository contains the charts for the mas api.
The repository has been configured to serve the static helm index and chart files

## Usage

```

$ helm repo add mas https://stephent2023.github.io/mas-api-helm/
"mas" has been added to your repositories

$ helm repo list 
NAME           	URL                               
mas           	https://stephent2023.github.io/mas-api-helm/

```

This API needs to be connected to a database to function. Do so by appending the following to helm install:
```
helm install api-container mas/mas-api --set DB_USER=... --set DB_PASS=... --set DB_NAME=... --set DB_ENDPOINT=...
```

Disable creation of ServiceAccounts by appending the following to helm install:
```

```
