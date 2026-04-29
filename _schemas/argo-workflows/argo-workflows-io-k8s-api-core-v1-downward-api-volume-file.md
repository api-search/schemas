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
source_filename: argo-workflows-io-k8s-api-core-v1-downward-api-volume-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-file-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.DownwardAPIVolumeFile\",\n  \"description\": \"DownwardAPIVolumeFile represents information to create the file containing the pod field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldRef\": {\n      \"description\": \"Required: Selects a field of the pod: only annotations, labels, name, namespace and uid are supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ObjectFieldSelector\"\n    },\n    \"mode\": {\n      \"description\": \"Optional: mode bits used to set permissions on this file, must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires decimal values for mode bits. If not specified,\
  \ the volume defaultMode will be used. This might be in conflict with other options that affect the file mode, like fsGroup, and the result can be other mode bits set.\",\n      \"type\": \"integer\"\n    },\n    \"path\": {\n      \"description\": \"Required: Path is  the relative path name of the file to be created. Must not be absolute or contain the '..' path. Must be utf-8 encoded. The first item of the relative path must not start with '..'\",\n      \"type\": \"string\"\n    },\n    \"resourceFieldRef\": {\n      \"description\": \"Selects a resource of the container: only resources limits and requests (limits.cpu, limits.memory, requests.cpu and requests.memory) are currently supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ResourceFieldSelector\"\n    }\n  },\n  \"required\": [\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-file-schema.json
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
