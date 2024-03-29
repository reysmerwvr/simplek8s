# simplek8s

> Kubernetes Sample With One Docker Container

## Requirements

- Kubernetes
- minikube >= 1.3.1
- kubectl >= 1.15.0

## Version

1.0.0

## Installation

Download zip file and extract it [latest pre-built release](https://github.com/reysmerwvr/simplek8s). Or clone the repository and cd into it.

This project uses a number of open source projects to work properly:

- [Kubernetes] - Production-Grade Container Orchestration

## Setup

Install kubectl and minikube for your OS.

[macOS](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-macos)
[Windows](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-windows)
[Linux](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-linux)

## Run minikube

```bash
hyperv
$ minikube start --vm-driver hyperv --hyperv-virtual-switch "<Minikube Name>"
virtualbox
$ minikube start –vm-driver=virtualbox -p <name>
hyperkit
$ minikube start --driver=hyperkit
```

Once running minikube

```bash
cd simplek8s
minikube status
kubectl cluster-info
kubectl apply -f client-pod.yaml
kubectl apply -f client-node.yaml
```

To verify pods/services status

```bash
cd simplek8s
kubectl get pods
kubectl get services
```

To verify minikube ip

```bash
cd simplek8s
minikube ip
```

## Contribute

We would love you for the contribution to **simplek8s**, check the ``LICENSE`` file for more info.

## TODO

- [ ] Write tests
- [ ] Add code comments

## Meta

Reysmer Valle – [@ReysmerWVR]

## License

Kubernetes Sample is (c) 2021 Reysmer Valle ([@ReysmerWVR]) and may be freely distributed under the [license-url]. See the `MIT-LICENSE` file.

[//]: # "These are reference links used in the body of this note and get stripped out when the markdown processor does
its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax"
[Kubernetes]: https://kubernetes.io/
