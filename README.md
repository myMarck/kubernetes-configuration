# Order
1. infrastructure
2. argocd(AppProject infrastructure)
3. sealed-secrets
4. kube-prometheus-stack
5. rook-ceph
6. rook-ceph-cluster
7. metallb
8. ingress-nginx
9. cert-manager
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