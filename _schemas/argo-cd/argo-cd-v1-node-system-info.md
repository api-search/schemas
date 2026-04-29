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
source_filename: argo-cd-v1-node-system-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-node-system-info-schema.json\",\n  \"title\": \"v1NodeSystemInfo\",\n  \"description\": \"NodeSystemInfo is a set of ids/uuids to uniquely identify the node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"architecture\": {\n      \"type\": \"string\",\n      \"title\": \"The Architecture reported by the node\"\n    },\n    \"bootID\": {\n      \"description\": \"Boot ID reported by the node.\",\n      \"type\": \"string\"\n    },\n    \"containerRuntimeVersion\": {\n      \"description\": \"ContainerRuntime Version reported by the node through runtime remote API (e.g. containerd://1.4.2).\",\n      \"type\": \"string\"\n    },\n    \"kernelVersion\": {\n      \"description\": \"Kernel Version reported by the node from 'uname -r' (e.g. 3.16.0-0.bpo.4-amd64).\",\n      \"type\": \"string\"\n\
  \    },\n    \"kubeProxyVersion\": {\n      \"description\": \"Deprecated: KubeProxy Version reported by the node.\",\n      \"type\": \"string\"\n    },\n    \"kubeletVersion\": {\n      \"description\": \"Kubelet Version reported by the node.\",\n      \"type\": \"string\"\n    },\n    \"machineID\": {\n      \"type\": \"string\",\n      \"title\": \"MachineID reported by the node. For unique machine identification\\nin the cluster this field is preferred. Learn more from man(5)\\nmachine-id: http://man7.org/linux/man-pages/man5/machine-id.5.html\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"title\": \"The Operating System reported by the node\"\n    },\n    \"osImage\": {\n      \"description\": \"OS Image reported by the node from /etc/os-release (e.g. Debian GNU/Linux 7 (wheezy)).\",\n      \"type\": \"string\"\n    },\n    \"swap\": {\n      \"$ref\": \"#/definitions/v1NodeSwapStatus\"\n    },\n    \"systemUUID\": {\n      \"type\": \"string\",\n   \
  \   \"title\": \"SystemUUID reported by the node. For unique machine identification\\nMachineID is preferred. This field is specific to Red Hat hosts\\nhttps://access.redhat.com/documentation/en-us/red_hat_subscription_management/1/html/rhsm/uuid\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-node-system-info-schema.json
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
