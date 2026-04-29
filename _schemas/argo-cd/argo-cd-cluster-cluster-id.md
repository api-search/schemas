---
description: clusterClusterID schema from Argo CD API
layout: schema
name: clusterClusterID
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-cluster-id-schema.json
slug: argo-cd-cluster-cluster-id
source_filename: argo-cd-cluster-cluster-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-cluster-id-schema.json\",\n  \"title\": \"clusterClusterID\",\n  \"description\": \"clusterClusterID schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"type is the type of the specified cluster identifier ( \\\"server\\\" - default, \\\"name\\\" )\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"title\": \"value holds the cluster server URL or cluster name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-cluster-id-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterClusterID
---
