---
description: ''
layout: schema
name: Authentication
properties_list:
- description: ''
  name: baseIdentityProvider
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: stripAuthorizationData
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-authentication-schema.json
slug: tyk-gateway-authentication
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Authentication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseIdentityProvider\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"stripAuthorizationData\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-authentication-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Authentication
---
