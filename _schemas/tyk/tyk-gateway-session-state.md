---
description: ''
layout: schema
name: SessionState
properties_list:
- description: ''
  name: access_rights
  type: object
- description: ''
  name: alias
  type: string
- description: ''
  name: allowance
  type: number
- description: ''
  name: apply_policies
  type: array
- description: deprecated use apply_policies going forward instead to send a list of policies ids
  name: apply_policy_id
  type: string
- description: ''
  name: certificate
  type: string
- description: ''
  name: data_expires
  type: integer
- description: ''
  name: date_created
  type: string
- description: deprecated use enable_detailed_recording going forward instead
  name: enable_detail_recording
  type: boolean
- description: ''
  name: enable_detailed_recording
  type: boolean
- description: ''
  name: enable_http_signature_validation
  type: boolean
- description: ''
  name: expires
  type: integer
- description: ''
  name: hmac_enabled
  type: boolean
- description: ''
  name: hmac_string
  type: string
- description: ''
  name: id_extractor_deadline
  type: integer
- description: ''
  name: is_inactive
  type: boolean
- description: ''
  name: last_check
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
  name: oauth_client_id
  type: string
- description: ''
  name: oauth_keys
  type: object
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
  name: rsa_certificate_id
  type: string
- description: ''
  name: session_lifetime
  type: integer
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
schema_file: json-schema/tyk-gateway-session-state-schema.json
slug: tyk-gateway-session-state
source_filename: tyk-gateway-session-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SessionState\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_rights\": {\n      \"type\": \"object\"\n    },\n    \"alias\": {\n      \"type\": \"string\"\n    },\n    \"allowance\": {\n      \"type\": \"number\"\n    },\n    \"apply_policies\": {\n      \"type\": \"array\"\n    },\n    \"apply_policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"deprecated use apply_policies going forward instead to send a list of policies ids\"\n    },\n    \"certificate\": {\n      \"type\": \"string\"\n    },\n    \"data_expires\": {\n      \"type\": \"integer\"\n    },\n    \"date_created\": {\n      \"type\": \"string\"\n    },\n    \"enable_detail_recording\": {\n      \"type\": \"boolean\",\n      \"description\": \"deprecated use enable_detailed_recording going forward instead\"\n    },\n    \"enable_detailed_recording\": {\n      \"type\": \"boolean\"\n    },\n    \"\
  enable_http_signature_validation\": {\n      \"type\": \"boolean\"\n    },\n    \"expires\": {\n      \"type\": \"integer\"\n    },\n    \"hmac_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"hmac_string\": {\n      \"type\": \"string\"\n    },\n    \"id_extractor_deadline\": {\n      \"type\": \"integer\"\n    },\n    \"is_inactive\": {\n      \"type\": \"boolean\"\n    },\n    \"last_check\": {\n      \"type\": \"integer\"\n    },\n    \"last_updated\": {\n      \"type\": \"string\"\n    },\n    \"max_query_depth\": {\n      \"type\": \"integer\"\n    },\n    \"meta_data\": {\n      \"type\": \"object\"\n    },\n    \"oauth_client_id\": {\n      \"type\": \"string\"\n    },\n    \"oauth_keys\": {\n      \"type\": \"object\"\n    },\n    \"org_id\": {\n      \"type\": \"string\"\n    },\n    \"per\": {\n      \"type\": \"number\"\n    },\n    \"quota_max\": {\n      \"type\": \"integer\"\n    },\n    \"quota_remaining\": {\n      \"type\": \"integer\"\n    },\n    \"quota_renewal_rate\"\
  : {\n      \"type\": \"integer\"\n    },\n    \"quota_renews\": {\n      \"type\": \"integer\"\n    },\n    \"rate\": {\n      \"type\": \"number\"\n    },\n    \"rsa_certificate_id\": {\n      \"type\": \"string\"\n    },\n    \"session_lifetime\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"throttle_interval\": {\n      \"type\": \"number\"\n    },\n    \"throttle_retry_limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-session-state-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: SessionState
---
