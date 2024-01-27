# kubectl-http - httpie krew plugin for kubectl

Call httpie with the credentials and the apiserver base URL of the current 
kubeconfig context.

## Install

1. Install [httpie](https://httpie.io/cli).
2. Install the [kubectl plugin manager krew](https://krew.sigs.k8s.io/)
2. Install this plugin: `kubectl krew install http`.

## Use

```shell
kubectl http --help
kubectl http -v /api/v1/namespaces/default/configmaps/foo
kubectl http put /api/v1/namespaces/default/configmaps/foo < configmap.yaml
```
