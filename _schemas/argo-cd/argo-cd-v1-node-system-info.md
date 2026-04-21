---
description: NodeSystemInfo is a set of ids/uuids to uniquely identify the node.
layout: schema
name: v1NodeSystemInfo
properties_list:
- description: ''
  name: architecture
  type: string
- description: Boot ID reported by the node.
  name: bootID
  type: string
- description: ContainerRuntime Version reported by the node through runtime remote API (e.g. containerd://1.4.2).
  name: containerRuntimeVersion
  type: string
- description: Kernel Version reported by the node from 'uname -r' (e.g. 3.16.0-0.bpo.4-amd64).
  name: kernelVersion
  type: string
- description: 'Deprecated: KubeProxy Version reported by the node.'
  name: kubeProxyVersion
  type: string
- description: Kubelet Version reported by the node.
  name: kubeletVersion
  type: string
- description: ''
  name: machineID
  type: string
- description: ''
  name: operatingSystem
  type: string
- description: OS Image reported by the node from /etc/os-release (e.g. Debian GNU/Linux 7 (wheezy)).
  name: osImage
  type: string
- description: ''
  name: swap
  type: object
- description: ''
  name: systemUUID
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-node-system-info-schema.json
slug: argo-cd-v1-node-system-info
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1NodeSystemInfo
---
