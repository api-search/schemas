---
description: Represents a projected volume source
layout: schema
name: io.k8s.api.core.v1.ProjectedVolumeSource
properties_list:
- description: defaultMode are the mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decima
  name: defaultMode
  type: integer
- description: sources is the list of volume projections. Each entry in this list handles one source.
  name: sources
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-projected-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-projected-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-projected-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-projected-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ProjectedVolumeSource\",\n  \"description\": \"Represents a projected volume source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultMode\": {\n      \"description\": \"defaultMode are the mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires decimal values for mode bits. Directories within the path are not affected by this setting. This might be in conflict with other options that affect the file mode, like fsGroup, and the result can be other mode bits set.\",\n      \"type\": \"integer\"\n    },\n    \"sources\": {\n      \"description\"\
  : \"sources is the list of volume projections. Each entry in this list handles one source.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.VolumeProjection\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-projected-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ProjectedVolumeSource
---
