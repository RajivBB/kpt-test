# kpt-test


kubectl create secret generic repo-creds-token \
  --namespace=dev-team \
  --from-literal=username=xxx \
  --from-literal=token=xxxx


kubectl create secret generic git-creds \
  --namespace=config-management-system \
  --from-literal=username=username \
  --from-literal=token=token

kubectl create secret generic git-creds \
  --namespace=prod-team \
  --from-literal=username=username \
  --from-literal=token=token
