---
description: Represents a host path mapped into a pod. Host path volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.HostPathVolumeSource
properties_list:
- description: 'path of the directory on the host. If the path is a symlink, it will follow the link to the real path. More info: https://kubernetes.io/docs/concepts/storage/volumes#hostpath'
  name: path
  type: string
- description: 'type for HostPath Volume Defaults to "" More info: https://kubernetes.io/docs/concepts/storage/volumes#hostpath'
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-host-path-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-host-path-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-host-path-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.HostPathVolumeSource\",\n  \"description\": \"Represents a host path mapped into a pod. Host path volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"description\": \"path of the directory on the host. If the path is a symlink, it will follow the link to the real path. More info: https://kubernetes.io/docs/concepts/storage/volumes#hostpath\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"type for HostPath Volume Defaults to \\\"\\\" More info: https://kubernetes.io/docs/concepts/storage/volumes#hostpath\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"path\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-host-path-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.HostPathVolumeSource
---
