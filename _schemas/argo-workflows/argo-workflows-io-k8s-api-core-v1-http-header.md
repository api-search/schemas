---
description: HTTPHeader describes a custom header to be used in HTTP probes
layout: schema
name: io.k8s.api.core.v1.HTTPHeader
properties_list:
- description: The header field name. This will be canonicalized upon output, so case-variant names will be understood as the same header.
  name: name
  type: string
- description: The header field value
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-http-header-schema.json
slug: argo-workflows-io-k8s-api-core-v1-http-header
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-http-header-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.HTTPHeader\",\n  \"description\": \"HTTPHeader describes a custom header to be used in HTTP probes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The header field name. This will be canonicalized upon output, so case-variant names will be understood as the same header.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The header field value\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-http-header-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.HTTPHeader
---
