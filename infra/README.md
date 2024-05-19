# README

## install

### local

#### cluster

kind is used in this document.

```bash:bash
❯ kind create cluster -n meta-controller --config cluster.yaml
```

#### meta controller

```bash:bash
❯ kubectl apply -k https://github.com/metacontroller/metacontroller/manifests/production
```

[link](https://metacontroller.github.io/metacontroller/guide/install.html)

#### application

* Image upload

```bash:bash

❯ kind load docker-image meta-controller-app(container image) -n kind-meta-controller

```

* Service apply

```bash:bash

❯ kubectl apply -k controller-app/

```

### EKS

TUB
