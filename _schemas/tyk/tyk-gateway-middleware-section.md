---
description: ''
layout: schema
name: MiddlewareSection
properties_list:
- description: ''
  name: driver
  type: string
- description: ''
  name: post
  type: array
- description: ''
  name: post_key_auth
  type: array
- description: ''
  name: pre
  type: array
- description: ''
  name: response
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-middleware-section-schema.json
slug: tyk-gateway-middleware-section
source_filename: tyk-gateway-middleware-section-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MiddlewareSection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"driver\": {\n      \"type\": \"string\"\n    },\n    \"post\": {\n      \"type\": \"array\"\n    },\n    \"post_key_auth\": {\n      \"type\": \"array\"\n    },\n    \"pre\": {\n      \"type\": \"array\"\n    },\n    \"response\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-middleware-section-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: MiddlewareSection
---
