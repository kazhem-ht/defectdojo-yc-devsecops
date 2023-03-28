# Personal helm charts

## Add repo
- To add repo:
    ```
    helm repo add kazhem-helm-charts https://kazhem-ht.github.io/helm-charts/
    ```
- Update repos
  ```
  helm repo update
  ```
- To check charts in added repo:
    ```
    helm search repo kazhem-helm-chart
    ```


## Add chart to repo
- Generate helm package from chart folder
  ```
  helm package .
  ```
- Copy generated `<chart_name>.tgz` to this repository dir
- Update index.yaml file on root of repository dir
  ```
  helm repo index .  --url "https://kazhem-ht.github.io/helm-charts/"
  ```
- Commit changes



## Current charts
```
❯ helm search repo kazhem-helm-chart
NAME                            CHART VERSION   APP VERSION     DESCRIPTION
kazhem-helm-charts/defectdojo   1.6.45          2.16.1          A Helm chart for Kubernetes to install DefectDojo
```
