# Getting Start with Tekton Pipeline on Kind(Kubernetes in Docker)
![](https://img.shields.io/badge/RHEL-8.5-blue?logo=redhat) ![](https://img.shields.io/badge/Docker-20.10.9-blue?logo=docker) ![](https://img.shields.io/badge/Kubernetes-v1.22.2-blue?logo=kubernetes) ![](https://img.shields.io/badge/Pipeline-v0.34.1-blue?logo=tekton)

Learning Tekton Pipeline Labs.

## Prerequisites
* An kind cluster.
* Installed Tekton from `akrade` or `helm`.
* Installed `kubectl` and `tkn` cli on your machine.

## How to getting cli tools
* [Arkade](https://github.com/alexellis/arkade): Recommended for people who are not used to linux environment configuration. 

```bash
# step 1: install arkade cli
$ curl -sLS https://get.arkade.dev | sudo sh
$ arkade --help

# step 2: chek the name of cli tool you need(ex: tkn)
$ arkade get --o table |grep tkn

# step 3: install need cli tool
$ akrade get tkn

# step 4: try tkn cli tool
$ export PATH=$PATH:$HOME/.arkade/bin/
$ tkn version
```

## How to install tekton
Now that you're all using `arkade`, let's keep using it. (ps: `helm` also works, but I'm not good at it)

```bash
# info: You must have a k8s first!
$ ark install tekton
$ kubectl get ns 
```




