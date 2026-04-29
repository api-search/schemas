---
description: Input schema for creating or updating a Consumer.
layout: schema
name: ConsumerInput
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: custom_id
  type: string
- description: ''
  name: tags
  type: array
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-consumer-input-schema.json
slug: kong-gateway-admin-consumer-input
source_filename: kong-gateway-admin-consumer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumerInput\",\n  \"type\": \"object\",\n  \"description\": \"Input schema for creating or updating a Consumer.\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"custom_id\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-consumer-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: ConsumerInput
---
