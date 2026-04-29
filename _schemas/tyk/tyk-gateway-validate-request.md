---
description: ''
layout: schema
name: ValidateRequest
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: errorResponseCode
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-validate-request-schema.json
slug: tyk-gateway-validate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"errorResponseCode\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-validate-request-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ValidateRequest
---
