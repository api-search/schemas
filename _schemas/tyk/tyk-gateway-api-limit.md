---
description: ''
layout: schema
name: APILimit
properties_list:
- description: ''
  name: max_query_depth
  type: integer
- description: ''
  name: per
  type: number
- description: ''
  name: quota_max
  type: integer
- description: ''
  name: quota_remaining
  type: integer
- description: ''
  name: quota_renewal_rate
  type: integer
- description: ''
  name: quota_renews
  type: integer
- description: ''
  name: rate
  type: number
- description: ''
  name: throttle_interval
  type: number
- description: ''
  name: throttle_retry_limit
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-api-limit-schema.json
slug: tyk-gateway-api-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"APILimit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"max_query_depth\": {\n      \"type\": \"integer\"\n    },\n    \"per\": {\n      \"type\": \"number\"\n    },\n    \"quota_max\": {\n      \"type\": \"integer\"\n    },\n    \"quota_remaining\": {\n      \"type\": \"integer\"\n    },\n    \"quota_renewal_rate\": {\n      \"type\": \"integer\"\n    },\n    \"quota_renews\": {\n      \"type\": \"integer\"\n    },\n    \"rate\": {\n      \"type\": \"number\"\n    },\n    \"throttle_interval\": {\n      \"type\": \"number\"\n    },\n    \"throttle_retry_limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-api-limit-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: APILimit
---
