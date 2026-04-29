---
description: A list of registered clusters.
layout: schema
name: ClusterList
properties_list:
- description: ''
  name: items
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-cluster-list-schema.json
slug: argo-cd-cluster-list
source_filename: argo-cd-cluster-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-cluster-list-schema.json\",\n  \"title\": \"ClusterList\",\n  \"description\": \"A list of registered clusters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Cluster\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-cluster-list-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ClusterList
---
