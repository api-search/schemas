---
description: ''
layout: schema
name: Introspection
properties_list:
- description: ''
  name: client_id
  type: string
- description: ''
  name: client_secret
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: identity_base_field
  type: string
- description: ''
  name: url
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-introspection-schema.json
slug: tyk-gateway-introspection
source_filename: tyk-gateway-introspection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Introspection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"identity_base_field\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-introspection-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Introspection
---
