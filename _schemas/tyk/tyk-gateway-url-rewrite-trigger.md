---
description: ''
layout: schema
name: URLRewriteTrigger
properties_list:
- description: ''
  name: condition
  type: string
- description: ''
  name: rewriteTo
  type: string
- description: ''
  name: rules
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-url-rewrite-trigger-schema.json
slug: tyk-gateway-url-rewrite-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"URLRewriteTrigger\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"type\": \"string\"\n    },\n    \"rewriteTo\": {\n      \"type\": \"string\"\n    },\n    \"rules\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-url-rewrite-trigger-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: URLRewriteTrigger
---
