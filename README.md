# prates-charts
Helm charts repository

 Execute:

helm repo add jetstack https://charts.jetstack.io
helm repo update
helm install cert-manager --create-namespace --namespace cert-manager --version v1.5.4 jetstack/cert-manager --set installCRDs=true --wait --debug

helm repo add prates-charts https://sergioprates.github.io/prates-charts/

helm install citus prates-charts/citus --debug --wait