---
description: ''
layout: schema
name: MiddlewareDefinition
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: raw_body_only
  type: boolean
- description: ''
  name: require_session
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-middleware-definition-schema.json
slug: tyk-gateway-middleware-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MiddlewareDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"raw_body_only\": {\n      \"type\": \"boolean\"\n    },\n    \"require_session\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-middleware-definition-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: MiddlewareDefinition
---
