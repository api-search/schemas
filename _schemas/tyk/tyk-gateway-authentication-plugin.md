---
description: ''
layout: schema
name: AuthenticationPlugin
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: functionName
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: rawBodyOnly
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-authentication-plugin-schema.json
slug: tyk-gateway-authentication-plugin
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthenticationPlugin\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"functionName\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"rawBodyOnly\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-authentication-plugin-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: AuthenticationPlugin
---
