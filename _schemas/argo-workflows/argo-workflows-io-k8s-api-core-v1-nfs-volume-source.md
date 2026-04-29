---
description: Represents an NFS mount that lasts the lifetime of a pod. NFS volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.NFSVolumeSource
properties_list:
- description: 'path that is exported by the NFS server. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs'
  name: path
  type: string
- description: 'readOnly here will force the NFS export to be mounted with read-only permissions. Defaults to false. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs'
  name: readOnly
  type: boolean
- description: 'server is the hostname or IP address of the NFS server. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs'
  name: server
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-nfs-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-nfs-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-nfs-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-nfs-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.NFSVolumeSource\",\n  \"description\": \"Represents an NFS mount that lasts the lifetime of a pod. NFS volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"description\": \"path that is exported by the NFS server. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly here will force the NFS export to be mounted with read-only permissions. Defaults to false. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs\",\n      \"type\": \"boolean\"\n    },\n    \"server\": {\n      \"description\": \"server\
  \ is the hostname or IP address of the NFS server. More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"server\",\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-nfs-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NFSVolumeSource
---
