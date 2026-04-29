---
description: ''
layout: schema
name: Policy
properties_list:
- description: ''
  name: _id
  type: string
- description: ''
  name: access_rights
  type: object
- description: ''
  name: active
  type: boolean
- description: ''
  name: enable_http_signature_validation
  type: boolean
- description: ''
  name: graphql_access_rights
  type: object
- description: ''
  name: hmac_enabled
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: is_inactive
  type: boolean
- description: ''
  name: key_expires_in
  type: integer
- description: ''
  name: last_updated
  type: string
- description: ''
  name: max_query_depth
  type: integer
- description: ''
  name: meta_data
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: org_id
  type: string
- description: ''
  name: per
  type: number
- description: ''
  name: quota_max
  type: integer
- description: ''
  name: quota_renewal_rate
  type: integer
- description: ''
  name: rate
  type: number
- description: ''
  name: tags
  type: array
- description: ''
  name: throttle_interval
  type: number
- description: ''
  name: throttle_retry_limit
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-policy-schema.json
slug: tyk-gateway-policy
source_filename: tyk-gateway-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Policy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\"\n    },\n    \"access_rights\": {\n      \"type\": \"object\"\n    },\n    \"active\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_http_signature_validation\": {\n      \"type\": \"boolean\"\n    },\n    \"graphql_access_rights\": {\n      \"type\": \"object\"\n    },\n    \"hmac_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"is_inactive\": {\n      \"type\": \"boolean\"\n    },\n    \"key_expires_in\": {\n      \"type\": \"integer\"\n    },\n    \"last_updated\": {\n      \"type\": \"string\"\n    },\n    \"max_query_depth\": {\n      \"type\": \"integer\"\n    },\n    \"meta_data\": {\n      \"type\": \"object\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"org_id\": {\n      \"type\": \"string\"\n  \
  \  },\n    \"per\": {\n      \"type\": \"number\"\n    },\n    \"quota_max\": {\n      \"type\": \"integer\"\n    },\n    \"quota_renewal_rate\": {\n      \"type\": \"integer\"\n    },\n    \"rate\": {\n      \"type\": \"number\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"throttle_interval\": {\n      \"type\": \"number\"\n    },\n    \"throttle_retry_limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-policy-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Policy
---
