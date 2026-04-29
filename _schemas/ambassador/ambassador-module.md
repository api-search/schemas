---
description: An Ambassador Module resource for configuring global Ambassador settings such as diagnostics, tracing, circuit breaking defaults, and retry policies.
layout: schema
name: Module
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-module-schema.json
slug: ambassador-module
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Module\",\n  \"type\": \"object\",\n  \"description\": \"An Ambassador Module resource for configuring global Ambassador settings such as diagnostics, tracing, circuit breaking defaults, and retry policies.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-module-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: Module
---
