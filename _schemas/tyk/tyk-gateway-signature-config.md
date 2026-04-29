---
description: ''
layout: schema
name: SignatureConfig
properties_list:
- description: ''
  name: algorithm
  type: string
- description: ''
  name: allowed_clock_skew
  type: integer
- description: ''
  name: error_code
  type: integer
- description: ''
  name: error_message
  type: string
- description: ''
  name: header
  type: string
- description: ''
  name: param_name
  type: string
- description: ''
  name: secret
  type: string
- description: ''
  name: use_param
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-signature-config-schema.json
slug: tyk-gateway-signature-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SignatureConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"algorithm\": {\n      \"type\": \"string\"\n    },\n    \"allowed_clock_skew\": {\n      \"type\": \"integer\"\n    },\n    \"error_code\": {\n      \"type\": \"integer\"\n    },\n    \"error_message\": {\n      \"type\": \"string\"\n    },\n    \"header\": {\n      \"type\": \"string\"\n    },\n    \"param_name\": {\n      \"type\": \"string\"\n    },\n    \"secret\": {\n      \"type\": \"string\"\n    },\n    \"use_param\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-signature-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: SignatureConfig
---
