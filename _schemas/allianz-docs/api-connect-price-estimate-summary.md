---
description: Summary information for a price estimate including status and premium
layout: schema
name: PriceEstimateSummary
properties_list:
- description: Unique identifier for the estimate
  name: estimate_id
  type: string
- description: Current status of the estimate
  name: status
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Annual premium amount
  name: annual_premium
  type: number
- description: Currency code
  name: currency
  type: string
- description: Timestamp when the estimate was created
  name: created_at
  type: string
- description: Date until which the estimate is valid
  name: valid_until
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-price-estimate-summary-schema.json
slug: api-connect-price-estimate-summary
source_filename: api-connect-price-estimate-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-summary-schema.json\",\n  \"title\": \"PriceEstimateSummary\",\n  \"description\": \"Summary information for a price estimate including status and premium\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the estimate\",\n      \"example\": \"est-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the estimate\",\n      \"enum\": [\n        \"active\",\n        \"expired\",\n        \"converted\"\n      ],\n      \"example\": \"active\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\",\n      \"example\": \"home\"\n    },\n    \"annual_premium\": {\n      \"type\"\
  : \"number\",\n      \"format\": \"double\",\n      \"description\": \"Annual premium amount\",\n      \"example\": 1250.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"AUD\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the estimate was created\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    },\n    \"valid_until\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date until which the estimate is valid\",\n      \"example\": \"2026-05-19\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-summary-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PriceEstimateSummary
---
