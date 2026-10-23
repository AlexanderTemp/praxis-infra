# platform

Cluster-wide pieces applied by hand with `kubectl apply -f` (not managed by Argo CD yet):
the public Gateway with its HTTPS listeners and the Let's Encrypt ClusterIssuer.
Kept here so the cluster can be rebuilt from Git. A new public hostname needs a listener in
`gateway.yaml`; cert-manager then issues its certificate.
