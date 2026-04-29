---
description: Health check configuration for an upstream.
layout: schema
name: Healthchecks
properties_list:
- description: ''
  name: active
  type: object
- description: ''
  name: passive
  type: object
- description: ''
  name: threshold
  type: number
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-healthchecks-schema.json
slug: kong-gateway-admin-healthchecks
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Healthchecks\",\n  \"type\": \"object\",\n  \"description\": \"Health check configuration for an upstream.\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"object\"\n    },\n    \"passive\": {\n      \"type\": \"object\"\n    },\n    \"threshold\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-healthchecks-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Healthchecks
---
