---
description: ''
layout: schema
name: TraceResponse
properties_list:
- description: ''
  name: logs
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: response
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-trace-response-schema.json
slug: tyk-gateway-trace-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TraceResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logs\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"response\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-trace-response-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: TraceResponse
---
