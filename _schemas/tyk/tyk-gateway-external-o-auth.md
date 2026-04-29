---
description: ''
layout: schema
name: ExternalOAuth
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: providers
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-external-o-auth-schema.json
slug: tyk-gateway-external-o-auth
source_filename: tyk-gateway-external-o-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExternalOAuth\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"providers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-external-o-auth-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ExternalOAuth
---
