# Order
### Wave 0 - 4
* infrastructure
* prometheus-operator-crds
* sealed-secrets
### Wave 5 - 9
* metallb
* ingress-nginx
### Wave 10 - 14
* cert-manager
### Wave 15 - 19
* cilium
* argocd
* rook-ceph
### Wave 20 - 24
* rook-ceph-cluster
### Manual order
1. kube-prometheus-stack
2. istio-base
3. istio-istiod
4. istio-cni
5. istio-ztunnel
6. istio-gateway
7. kiali-operator

# Manuel steps
https://grafana.com/docs/grafana/latest/administration/service-accounts/#create-a-service-account-in-grafana

kubectl -n kiali-operator create secret generic grafana-access --from-literal=token-viewer=< token >