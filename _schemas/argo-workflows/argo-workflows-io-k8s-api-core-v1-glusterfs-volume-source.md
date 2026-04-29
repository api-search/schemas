---
description: Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.GlusterfsVolumeSource
properties_list:
- description: endpoints is the endpoint name that details Glusterfs topology.
  name: endpoints
  type: string
- description: 'path is the Glusterfs volume path. More info: https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod'
  name: path
  type: string
- description: 'readOnly here will force the Glusterfs volume to be mounted with read-only permissions. Defaults to false. More info: https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod'
  name: readOnly
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-glusterfs-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-glusterfs-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-glusterfs-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.GlusterfsVolumeSource\",\n  \"description\": \"Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoints\": {\n      \"description\": \"endpoints is the endpoint name that details Glusterfs topology.\",\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"description\": \"path is the Glusterfs volume path. More info: https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly here will force the Glusterfs volume to be mounted with read-only permissions.\
  \ Defaults to false. More info: https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"endpoints\",\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-glusterfs-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.GlusterfsVolumeSource
---
