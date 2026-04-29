---
description: ''
layout: schema
name: TargetInput
properties_list:
- description: The target address (IP or hostname) and port.
  name: target
  type: string
- description: ''
  name: weight
  type: integer
- description: ''
  name: tags
  type: array
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-target-input-schema.json
slug: kong-gateway-admin-target-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The target address (IP or hostname) and port.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-target-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: TargetInput
---
