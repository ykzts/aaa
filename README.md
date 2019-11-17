# Graph

## Requirements

- [`kubectl`](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [`kustomize`](https://github.com/kubernetes-sigs/kustomize/releases)
- [`skaffold`](https://skaffold.dev/docs/install/)

## Deploy


```console
$ kubectl create secret generic twitter-credentials \
  --from-literal=access-token=... --from-literal=access-token-secret=... \
  --from-literal=consumer-key=... --from-literal=consumer-secret=...
$ kubectl create secret generic azure-blob-credentials \
  --from-literal=account-name=... --from-literal=account-key=... \
  --from-literal=container-name=...
$ skaffold run -p production
```

## License

[MIT](LICENSE)
