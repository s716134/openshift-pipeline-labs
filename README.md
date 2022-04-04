# Getting Start with Tekton Pipeline on Kind(Kubernetes in Docker)
![](https://img.shields.io/badge/RHEL-8.5-blue?logo=redhat) ![](https://img.shields.io/badge/Docker-20.10.9-blue?logo=docker) ![](https://img.shields.io/badge/Kubernetes-v1.22.2-blue?logo=kubernetes) ![](https://img.shields.io/badge/Pipeline-v0.34.1-blue?logo=tekton)

Learning Tekton Pipeline Labs.

## Prerequisites
* An kind cluster.
* Installed Tekton from `akrade` or `helm`.
* Installed `kubectl` and `tkn` CLI on your machine.

## How to Install CLI tools
* [Arkade](https://github.com/alexellis/arkade): Recommended for people who are not used to linux environment configuration: 

```bash
# step 1: install arkade CLI
$ curl -sLS https://get.arkade.dev | sudo sh
$ arkade --help

# step 2: cheking you need CLI tool(ex: tkn)
$ arkade get --o table |grep tkn

# step 3: install need CLI
$ akrade get tkn

# step 4: try tkn CLI
$ export PATH=$PATH:$HOME/.arkade/bin/
$ tkn version
```
