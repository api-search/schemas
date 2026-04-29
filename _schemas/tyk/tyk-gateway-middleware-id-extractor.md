---
description: ''
layout: schema
name: MiddlewareIdExtractor
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: extract_from
  type: string
- description: ''
  name: extract_with
  type: string
- description: ''
  name: extractor_config
  type: object
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-middleware-id-extractor-schema.json
slug: tyk-gateway-middleware-id-extractor
source_filename: tyk-gateway-middleware-id-extractor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MiddlewareIdExtractor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"extract_from\": {\n      \"type\": \"string\"\n    },\n    \"extract_with\": {\n      \"type\": \"string\"\n    },\n    \"extractor_config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-middleware-id-extractor-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: MiddlewareIdExtractor
---
