---
description: ''
layout: schema
name: OAuthClientToken
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: expires
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-o-auth-client-token-schema.json
slug: tyk-gateway-o-auth-client-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OAuthClientToken\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"expires\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-o-auth-client-token-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: OAuthClientToken
---
