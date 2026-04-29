---
description: ''
layout: schema
name: VirtualEndpoint
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: functionName
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: proxyOnError
  type: boolean
- description: ''
  name: requireSession
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-virtual-endpoint-schema.json
slug: tyk-gateway-virtual-endpoint
source_filename: tyk-gateway-virtual-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualEndpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"functionName\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"proxyOnError\": {\n      \"type\": \"boolean\"\n    },\n    \"requireSession\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-virtual-endpoint-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: VirtualEndpoint
---
