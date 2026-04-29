---
description: Represents downward API info for projecting into a projected volume. Note that this is identical to a downwardAPI volume source without the default mode.
layout: schema
name: io.k8s.api.core.v1.DownwardAPIProjection
properties_list:
- description: Items is a list of DownwardAPIVolume file
  name: items
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-projection-schema.json
slug: argo-workflows-io-k8s-api-core-v1-downward-api-projection
source_filename: argo-workflows-io-k8s-api-core-v1-downward-api-projection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-projection-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.DownwardAPIProjection\",\n  \"description\": \"Represents downward API info for projecting into a projected volume. Note that this is identical to a downwardAPI volume source without the default mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"description\": \"Items is a list of DownwardAPIVolume file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.DownwardAPIVolumeFile\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-downward-api-projection-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.DownwardAPIProjection
---
