---
description: DownwardAPIVolumeFile represents information to create the file containing the pod field
layout: schema
name: io.k8s.api.core.v1.DownwardAPIVolumeFile
properties_list:
- description: 'Required: Selects a field of the pod: only annotations, labels, name, namespace and uid are supported.'
  name: fieldRef
  type: object
- description: 'Optional: mode bits used to set permissions on this file, must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires d'
  name: mode
  type: integer
- description: 'Required: Path is the relative path name of the file to be created. Must not be absolute or contain the ''..'' path. Must be utf-8 encoded. The first item of the relative path must not start with ''..'''
  name: path
  type: string
- description: 'Selects a resource of the container: only resources limits and requests (limits.cpu, limits.memory, requests.cpu and requests.memory) are currently supported.'
  name: resourceFieldRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-file-schema.json
slug: argo-workflows-io-k8s-api-core-v1-downward-api-volume-file
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.DownwardAPIVolumeFile
---
