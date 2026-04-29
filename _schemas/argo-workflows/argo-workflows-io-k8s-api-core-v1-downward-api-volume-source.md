---
description: DownwardAPIVolumeSource represents a volume containing downward API info. Downward API volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.DownwardAPIVolumeSource
properties_list:
- description: 'Optional: mode bits to use on created files by default. Must be a Optional: mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal val'
  name: defaultMode
  type: integer
- description: Items is a list of downward API volume file
  name: items
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-downward-api-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-downward-api-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.DownwardAPIVolumeSource\",\n  \"description\": \"DownwardAPIVolumeSource represents a volume containing downward API info. Downward API volumes support ownership management and SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultMode\": {\n      \"description\": \"Optional: mode bits to use on created files by default. Must be a Optional: mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires decimal values for mode bits. Defaults to 0644. Directories within the path are not affected by this setting. This might be in\
  \ conflict with other options that affect the file mode, like fsGroup, and the result can be other mode bits set.\",\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"description\": \"Items is a list of downward API volume file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.DownwardAPIVolumeFile\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.DownwardAPIVolumeSource
---
