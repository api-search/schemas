---
description: ''
layout: schema
name: Domain
properties_list:
- description: ''
  name: certificates
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: name
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-domain-schema.json
slug: tyk-gateway-domain
source_filename: tyk-gateway-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Domain\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificates\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-domain-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Domain
---
