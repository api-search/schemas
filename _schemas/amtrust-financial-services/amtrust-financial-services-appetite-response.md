---
description: Coverage appetite check result
layout: schema
name: AppetiteResponse
properties_list:
- description: Whether AmTrust has appetite for this risk
  name: eligible
  type: boolean
- description: Available products for this risk
  name: products
  type: array
- description: Whether the policy can be bound online
  name: bind_online
  type: boolean
- description: Reason if not eligible
  name: reason
  type: string
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-appetite-response-schema.json
slug: amtrust-financial-services-appetite-response
source_filename: amtrust-financial-services-appetite-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-appetite-response-schema.json\",\n  \"title\": \"AppetiteResponse\",\n  \"description\": \"Coverage appetite check result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eligible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AmTrust has appetite for this risk\",\n      \"example\": true\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"Available products for this risk\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"workers_compensation\"\n      ]\n    },\n    \"bind_online\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy can be bound online\",\n      \"example\": true\n    },\n    \"reason\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Reason if not eligible\",\n      \"example\": \"Eligible for online quoting and binding\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-appetite-response-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: AppetiteResponse
---
