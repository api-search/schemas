---
description: ''
layout: schema
name: IDExtractorConfig
properties_list:
- description: ''
  name: formParamName
  type: string
- description: ''
  name: headerName
  type: string
- description: ''
  name: regexp
  type: string
- description: ''
  name: regexpMatchIndex
  type: integer
- description: ''
  name: xPathExp
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-id-extractor-config-schema.json
slug: tyk-gateway-id-extractor-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IDExtractorConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formParamName\": {\n      \"type\": \"string\"\n    },\n    \"headerName\": {\n      \"type\": \"string\"\n    },\n    \"regexp\": {\n      \"type\": \"string\"\n    },\n    \"regexpMatchIndex\": {\n      \"type\": \"integer\"\n    },\n    \"xPathExp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-id-extractor-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: IDExtractorConfig
---
