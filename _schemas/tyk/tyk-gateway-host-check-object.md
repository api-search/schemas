---
description: ''
layout: schema
name: HostCheckObject
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: commands
  type: array
- description: ''
  name: enable_proxy_protocol
  type: boolean
- description: ''
  name: headers
  type: object
- description: ''
  name: method
  type: string
- description: ''
  name: protocol
  type: string
- description: ''
  name: timeout
  type: integer
- description: ''
  name: url
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-host-check-object-schema.json
slug: tyk-gateway-host-check-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostCheckObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"commands\": {\n      \"type\": \"array\"\n    },\n    \"enable_proxy_protocol\": {\n      \"type\": \"boolean\"\n    },\n    \"headers\": {\n      \"type\": \"object\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"protocol\": {\n      \"type\": \"string\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-host-check-object-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: HostCheckObject
---
