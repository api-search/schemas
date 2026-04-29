---
description: ''
layout: schema
name: TraceHttpRequest
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-trace-http-request-schema.json
slug: tyk-gateway-trace-http-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TraceHttpRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-trace-http-request-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: TraceHttpRequest
---
