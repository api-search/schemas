---
description: ''
layout: schema
name: RequestSigningMeta
properties_list:
- description: ''
  name: algorithm
  type: string
- description: ''
  name: certificate_id
  type: string
- description: ''
  name: header_list
  type: array
- description: ''
  name: is_enabled
  type: boolean
- description: ''
  name: key_id
  type: string
- description: ''
  name: secret
  type: string
- description: ''
  name: signature_header
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-request-signing-meta-schema.json
slug: tyk-gateway-request-signing-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestSigningMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"algorithm\": {\n      \"type\": \"string\"\n    },\n    \"certificate_id\": {\n      \"type\": \"string\"\n    },\n    \"header_list\": {\n      \"type\": \"array\"\n    },\n    \"is_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"key_id\": {\n      \"type\": \"string\"\n    },\n    \"secret\": {\n      \"type\": \"string\"\n    },\n    \"signature_header\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-request-signing-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RequestSigningMeta
---
