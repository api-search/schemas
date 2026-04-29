---
description: Sysctl defines a kernel parameter to be set
layout: schema
name: io.k8s.api.core.v1.Sysctl
properties_list:
- description: Name of a property to set
  name: name
  type: string
- description: Value of a property to set
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-sysctl-schema.json
slug: argo-workflows-io-k8s-api-core-v1-sysctl
source_filename: argo-workflows-io-k8s-api-core-v1-sysctl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-sysctl-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Sysctl\",\n  \"description\": \"Sysctl defines a kernel parameter to be set\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of a property to set\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Value of a property to set\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-sysctl-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Sysctl
---
