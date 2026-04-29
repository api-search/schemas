---
description: ''
layout: schema
name: RequestDefinition
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: headers
  type: object
- description: ''
  name: method
  type: string
- description: ''
  name: relative_url
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-request-definition-schema.json
slug: tyk-gateway-request-definition
source_filename: tyk-gateway-request-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"headers\": {\n      \"type\": \"object\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"relative_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-request-definition-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RequestDefinition
---
