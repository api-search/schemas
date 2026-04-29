---
description: ''
layout: schema
name: RoutingTrigger
properties_list:
- description: ''
  name: 'on'
  type: string
- description: ''
  name: rewrite_to
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-routing-trigger-schema.json
slug: tyk-gateway-routing-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutingTrigger\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"on\": {\n      \"type\": \"string\"\n    },\n    \"rewrite_to\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-routing-trigger-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RoutingTrigger
---
