# sk026 Helm chart repository

Class: `class-1` · Student: `sk026`

```sh
helm repo add sk026-github https://hyunooss.github.io/mycharts
helm repo update sk026-github
helm search repo sk026-github/sk026-myfirst-helmchart --versions
helm upgrade --install sk026-myfirst-helm sk026-github/sk026-myfirst-helmchart \
  --version 0.0.2 --namespace class-1 --rollback-on-failure --wait --timeout 3m
```

The namespace must already contain the student imagePullSecret `sk026-helm-registry`.
0.0.1: application 1.0, 1 replica. 0.0.2: application 2.0, 2 replicas.
