---
description: Adds and removes POSIX capabilities from running containers.
layout: schema
name: io.k8s.api.core.v1.Capabilities
properties_list:
- description: Added capabilities
  name: add
  type: array
- description: Removed capabilities
  name: drop
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-capabilities-schema.json
slug: argo-workflows-io-k8s-api-core-v1-capabilities
source_filename: argo-workflows-io-k8s-api-core-v1-capabilities-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-capabilities-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Capabilities\",\n  \"description\": \"Adds and removes POSIX capabilities from running containers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"add\": {\n      \"description\": \"Added capabilities\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"drop\": {\n      \"description\": \"Removed capabilities\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-capabilities-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Capabilities
---
