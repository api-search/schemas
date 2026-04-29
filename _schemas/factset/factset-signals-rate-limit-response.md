---
description: Error returned if any of the user's rate limit have been reached.
layout: schema
name: rateLimitResponse
properties_list:
- description: ''
  name: message
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-rate-limit-response-schema.json
slug: factset-signals-rate-limit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"rateLimitResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error returned if any of the user's rate limit have been reached.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-rate-limit-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: rateLimitResponse
---
