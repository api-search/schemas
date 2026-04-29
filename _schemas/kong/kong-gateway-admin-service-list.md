---
description: A paginated list of Service entities.
layout: schema
name: ServiceList
properties_list:
- description: ''
  name: data
  type: array
- description: URI to the next page of results.
  name: next
  type: string
- description: Offset token for the next page.
  name: offset
  type: string
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-service-list-schema.json
slug: kong-gateway-admin-service-list
source_filename: kong-gateway-admin-service-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of Service entities.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"URI to the next page of results.\"\n    },\n    \"offset\": {\n      \"type\": \"string\",\n      \"description\": \"Offset token for the next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-service-list-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: ServiceList
---
