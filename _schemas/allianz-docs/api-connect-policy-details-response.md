---
description: Policy details and quote ready for binding
layout: schema
name: PolicyDetailsResponse
properties_list:
- description: Unique identifier for the completed quote
  name: quote_id
  type: string
- description: Assigned policy number
  name: policy_number
  type: string
- description: Status of the policy quote
  name: status
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Annual premium for the policy
  name: annual_premium
  type: number
- description: Currency code
  name: currency
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-policy-details-response-schema.json
slug: api-connect-policy-details-response
source_filename: api-connect-policy-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-response-schema.json\",\n  \"title\": \"PolicyDetailsResponse\",\n  \"description\": \"Policy details and quote ready for binding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quote_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the completed quote\",\n      \"example\": \"quote-500567\"\n    },\n    \"policy_number\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned policy number\",\n      \"example\": \"ALZ-2026-500567\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the policy quote\",\n      \"enum\": [\n        \"ready_to_bind\",\n        \"pending\",\n        \"bound\"\n      ],\n      \"example\": \"ready_to_bind\"\n    },\n    \"product_type\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Insurance product type\",\n      \"example\": \"home\"\n    },\n    \"annual_premium\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Annual premium for the policy\",\n      \"example\": 1250.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"AUD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PolicyDetailsResponse
---
