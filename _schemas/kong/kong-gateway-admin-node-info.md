---
description: General details about the Kong Gateway node.
layout: schema
name: NodeInfo
properties_list:
- description: The version of the Kong Gateway instance.
  name: version
  type: string
- description: The version of the Lua runtime.
  name: lua_version
  type: string
- description: ''
  name: tagline
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: timers
  type: object
- description: ''
  name: plugins
  type: object
- description: ''
  name: configuration
  type: object
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-node-info-schema.json
slug: kong-gateway-admin-node-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NodeInfo\",\n  \"type\": \"object\",\n  \"description\": \"General details about the Kong Gateway node.\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Kong Gateway instance.\"\n    },\n    \"lua_version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Lua runtime.\"\n    },\n    \"tagline\": {\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"timers\": {\n      \"type\": \"object\"\n    },\n    \"plugins\": {\n      \"type\": \"object\"\n    },\n    \"configuration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-node-info-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: NodeInfo
---
