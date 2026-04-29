---
description: ''
layout: schema
name: EventHandler
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: trigger
  type: string
- description: ''
  name: type
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-event-handler-schema.json
slug: tyk-gateway-event-handler
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventHandler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"trigger\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-event-handler-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: EventHandler
---
