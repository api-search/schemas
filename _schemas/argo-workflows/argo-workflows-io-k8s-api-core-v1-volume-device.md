---
description: volumeDevice describes a mapping of a raw block device within a container.
layout: schema
name: io.k8s.api.core.v1.VolumeDevice
properties_list:
- description: devicePath is the path inside of the container that the device will be mapped to.
  name: devicePath
  type: string
- description: name must match the name of a persistentVolumeClaim in the pod
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-device-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume-device
source_filename: argo-workflows-io-k8s-api-core-v1-volume-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-device-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.VolumeDevice\",\n  \"description\": \"volumeDevice describes a mapping of a raw block device within a container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"devicePath\": {\n      \"description\": \"devicePath is the path inside of the container that the device will be mapped to.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"name must match the name of a persistentVolumeClaim in the pod\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"devicePath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-device-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VolumeDevice
---
