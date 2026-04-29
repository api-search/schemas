---
description: Price estimate result with premium amounts
layout: schema
name: PriceEstimateResponse
properties_list:
- description: Unique identifier for the generated estimate
  name: estimate_id
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Annual insurance premium amount
  name: annual_premium
  type: number
- description: Monthly insurance premium amount
  name: monthly_premium
  type: number
- description: Currency code for the premium amounts
  name: currency
  type: string
- description: Date until which this estimate is valid
  name: valid_until
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-price-estimate-response-schema.json
slug: api-connect-price-estimate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-response-schema.json\",\n  \"title\": \"PriceEstimateResponse\",\n  \"description\": \"Price estimate result with premium amounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the generated estimate\",\n      \"example\": \"est-500123\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\",\n      \"example\": \"home\"\n    },\n    \"annual_premium\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Annual insurance premium amount\",\n      \"example\": 1250.0\n    },\n    \"monthly_premium\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"\
  Monthly insurance premium amount\",\n      \"example\": 104.17\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for the premium amounts\",\n      \"example\": \"AUD\"\n    },\n    \"valid_until\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date until which this estimate is valid\",\n      \"example\": \"2026-05-19\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PriceEstimateResponse
---
