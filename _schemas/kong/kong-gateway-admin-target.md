---
description: A Target is an IP address/hostname with a port that identifies an instance of a backend service.
layout: schema
name: Target
properties_list:
- description: ''
  name: id
  type: string
- description: The target address (IP or hostname) and port (host:port).
  name: target
  type: string
- description: The weight this target gets within the upstream (0-65535). 0 means the target is disabled.
  name: weight
  type: integer
- description: ''
  name: tags
  type: array
- description: ''
  name: upstream
  type: object
- description: ''
  name: created_at
  type: number
- description: ''
  name: updated_at
  type: number
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-target-schema.json
slug: kong-gateway-admin-target
source_filename: kong-gateway-admin-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Target\",\n  \"type\": \"object\",\n  \"description\": \"A Target is an IP address/hostname with a port that identifies an instance of a backend service.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The target address (IP or hostname) and port (host:port).\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The weight this target gets within the upstream (0-65535). 0 means the target is disabled.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"upstream\": {\n      \"type\": \"object\"\n    },\n    \"created_at\": {\n      \"type\": \"number\"\n    },\n    \"updated_at\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-target-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Target
---
