---
description: Status information about the Kong Gateway node.
layout: schema
name: NodeStatus
properties_list:
- description: ''
  name: database
  type: object
- description: ''
  name: memory
  type: object
- description: ''
  name: server
  type: object
- description: ''
  name: configuration_hash
  type: string
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-node-status-schema.json
slug: kong-gateway-admin-node-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NodeStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status information about the Kong Gateway node.\",\n  \"properties\": {\n    \"database\": {\n      \"type\": \"object\"\n    },\n    \"memory\": {\n      \"type\": \"object\"\n    },\n    \"server\": {\n      \"type\": \"object\"\n    },\n    \"configuration_hash\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-node-status-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: NodeStatus
---
