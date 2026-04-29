---
description: ResourceFieldSelector represents container resources (cpu, memory) and their output format
layout: schema
name: io.k8s.api.core.v1.ResourceFieldSelector
properties_list:
- description: 'Container name: required for volumes, optional for env vars'
  name: containerName
  type: string
- description: Specifies the output format of the exposed resources, defaults to "1"
  name: divisor
  type: object
- description: 'Required: resource to select'
  name: resource
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-resource-field-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-resource-field-selector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-resource-field-selector-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ResourceFieldSelector\",\n  \"description\": \"ResourceFieldSelector represents container resources (cpu, memory) and their output format\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containerName\": {\n      \"description\": \"Container name: required for volumes, optional for env vars\",\n      \"type\": \"string\"\n    },\n    \"divisor\": {\n      \"description\": \"Specifies the output format of the exposed resources, defaults to \\\"1\\\"\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\n    },\n    \"resource\": {\n      \"description\": \"Required: resource to select\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"resource\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-resource-field-selector-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ResourceFieldSelector
---
