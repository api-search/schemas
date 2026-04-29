---
description: ''
layout: schema
name: RateLimit
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: per
  type: integer
- description: ''
  name: rate
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-rate-limit-schema.json
slug: tyk-gateway-rate-limit
source_filename: tyk-gateway-rate-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"per\": {\n      \"type\": \"integer\"\n    },\n    \"rate\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-rate-limit-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RateLimit
---
