---
description: ''
layout: schema
name: ValidateRequestMeta
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: error_response_code
  type: integer
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-validate-request-meta-schema.json
slug: tyk-gateway-validate-request-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidateRequestMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"error_response_code\": {\n      \"type\": \"integer\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-validate-request-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ValidateRequestMeta
---
