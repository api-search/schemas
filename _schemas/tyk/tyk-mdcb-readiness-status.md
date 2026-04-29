---
description: ''
layout: schema
name: ReadinessStatus
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: status_code
  type: integer
- description: ''
  name: components
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-mdcb-readiness-status-schema.json
slug: tyk-mdcb-readiness-status
source_filename: tyk-mdcb-readiness-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReadinessStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"status_code\": {\n      \"type\": \"integer\"\n    },\n    \"components\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-mdcb-readiness-status-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ReadinessStatus
---
