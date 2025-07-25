
kubectl create secret generic git-creds \
  --namespace=config-management-system \
  --from-literal=username=rajivbb \
  --from-literal=token=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


kubectl create secret generic git-creds \
  --namespace=prod-team \
  --from-literal=username=rajibb \
  --from-literal=token=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


ssh

kubectl create secret generic repo-creds-ssh   --namespace=config-management-system  --from-file=ssh-privatekey=/home/rsingh/.ssh/id_ed25519  --context kind-east

kubectl create secret generic repo-creds-ssh   --namespace=prod-team  --from-file=ssh-privatekey=/home/rsingh/.ssh/id_ed25519  --context kind-east

