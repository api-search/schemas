---
description: ''
layout: schema
name: BatchRequestStructure
properties_list:
- description: ''
  name: requests
  type: array
- description: ''
  name: suppress_parallel_execution
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-batch-request-structure-schema.json
slug: tyk-gateway-batch-request-structure
source_filename: tyk-gateway-batch-request-structure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchRequestStructure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requests\": {\n      \"type\": \"array\"\n    },\n    \"suppress_parallel_execution\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-batch-request-structure-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: BatchRequestStructure
---
