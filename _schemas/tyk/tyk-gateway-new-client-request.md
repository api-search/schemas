---
description: ''
layout: schema
name: NewClientRequest
properties_list:
- description: ''
  name: api_id
  type: string
- description: ''
  name: client_id
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: meta_data
  type: object
- description: ''
  name: policy_id
  type: string
- description: ''
  name: redirect_uri
  type: string
- description: ''
  name: secret
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-new-client-request-schema.json
slug: tyk-gateway-new-client-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NewClientRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_id\": {\n      \"type\": \"string\"\n    },\n    \"client_id\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"meta_data\": {\n      \"type\": \"object\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\"\n    },\n    \"redirect_uri\": {\n      \"type\": \"string\"\n    },\n    \"secret\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-new-client-request-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: NewClientRequest
---
