# Order
### Wave 0 - 4
* infrastructure
* prometheus-operator-crds
### Wave 5 - 9
* sealed-secrets
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
* k8s-monitoring

### Manual order
2. istio-base
3. istio-istiod
4. istio-cni
5. istio-ztunnel
6. istio-gateway
7. kiali-operator

# Manuel steps
https://grafana.com/docs/grafana/latest/administration/service-accounts/#create-a-service-account-in-grafana

kubectl -n kiali-operator create secret generic grafana-access --from-literal=token-viewer=< token >

# third party
In auth0.com
Actions -> triggers
post-login
Custom role -> addRoles
```
exports.onExecutePostLogin = async (event, api) => {
  const namespace = 'https://odumsborg.dk';
  if (event.authorization) {
    api.idToken.setCustomClaim(`${namespace}/roles`, event.authorization.roles);
    api.accessToken.setCustomClaim(`${namespace}/roles`, event.authorization.roles);
  }
}
```