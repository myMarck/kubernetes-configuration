# Order
1. infrastructure
2. prometheus-operator-crds
3. sealed-secrets
4. metallb
5. ingress-nginx
6. cert-manager
7. kube-prometheus-stack
8. rook-ceph
9. rook-ceph-cluster
10. cilium
11. argocd
12. istio-base
13. istio-istiod
14. istio-cni
15. istio-ztunnel
16. istio-gateway
17. kiali-operator

# Manuel steps
https://grafana.com/docs/grafana/latest/administration/service-accounts/#create-a-service-account-in-grafana

kubectl -n kiali-operator create secret generic grafana-access --from-literal=token-viewer=< token >