---
description: Bound policy details
layout: schema
name: PolicyResponse
properties_list:
- description: Unique AmTrust policy number
  name: policy_number
  type: string
- description: Policy status
  name: status
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Annual premium
  name: premium
  type: number
- description: ''
  name: effective_date
  type: string
- description: ''
  name: expiration_date
  type: string
- description: ''
  name: insured
  type: object
- description: ''
  name: bound_at
  type: string
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-policy-response-schema.json
slug: amtrust-financial-services-policy-response
source_filename: amtrust-financial-services-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-policy-response-schema.json\",\n  \"title\": \"PolicyResponse\",\n  \"description\": \"Bound policy details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_number\": {\n      \"type\": \"string\",\n      \"description\": \"Unique AmTrust policy number\",\n      \"example\": \"WC-2025-001234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Policy status\",\n      \"enum\": [\n        \"active\",\n        \"cancelled\",\n        \"expired\"\n      ],\n      \"example\": \"active\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\",\n      \"example\": \"workers_compensation\"\n    },\n    \"premium\": {\n      \"type\": \"number\",\n      \"description\": \"\
  Annual premium\",\n      \"example\": 8250.0\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-07-01\"\n    },\n    \"expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2026-07-01\"\n    },\n    \"insured\": {\n      \"$ref\": \"#/components/schemas/Insured\"\n    },\n    \"bound_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T15:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-policy-response-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: PolicyResponse
---
