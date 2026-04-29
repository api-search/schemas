---
description: ''
layout: schema
name: IDExtractor
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: source
  type: string
- description: ''
  name: with
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-id-extractor-schema.json
slug: tyk-gateway-id-extractor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IDExtractor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"with\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-id-extractor-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: IDExtractor
---
