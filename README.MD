## Grafana admin account admin decode

kubectl get secret --namespace default my-release-grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo

kubectl get secret --namespace default my-prometheus-grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo