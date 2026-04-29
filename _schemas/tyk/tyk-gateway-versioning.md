---
description: ''
layout: schema
name: Versioning
properties_list:
- description: ''
  name: default
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: fallbackToDefault
  type: boolean
- description: ''
  name: key
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: stripVersioningData
  type: boolean
- description: ''
  name: urlVersioningPattern
  type: string
- description: ''
  name: versions
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-versioning-schema.json
slug: tyk-gateway-versioning
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Versioning\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"fallbackToDefault\": {\n      \"type\": \"boolean\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"stripVersioningData\": {\n      \"type\": \"boolean\"\n    },\n    \"urlVersioningPattern\": {\n      \"type\": \"string\"\n    },\n    \"versions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-versioning-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Versioning
---
