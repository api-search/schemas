---
description: A paginated list of Consumer entities.
layout: schema
name: ConsumerList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: next
  type: string
- description: ''
  name: offset
  type: string
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-consumer-list-schema.json
slug: kong-gateway-admin-consumer-list
source_filename: kong-gateway-admin-consumer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumerList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of Consumer entities.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"offset\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-consumer-list-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: ConsumerList
---
