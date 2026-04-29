---
description: ''
layout: schema
name: OIDC
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: providers
  type: array
- description: ''
  name: segregateByClientId
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-oidc-schema.json
slug: tyk-gateway-oidc
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OIDC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"providers\": {\n      \"type\": \"array\"\n    },\n    \"segregateByClientId\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-oidc-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: OIDC
---
