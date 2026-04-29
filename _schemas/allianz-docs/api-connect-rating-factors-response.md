---
description: Detailed premium breakdown and rating factors for an estimate
layout: schema
name: RatingFactorsResponse
properties_list:
- description: Unique identifier for the estimate
  name: estimate_id
  type: string
- description: Base premium before adjustments
  name: base_premium
  type: number
- description: Additional risk-based premium loading
  name: risk_loading
  type: number
- description: Applied discounts
  name: discounts
  type: number
- description: Government stamp duty
  name: stamp_duty
  type: number
- description: Final annual premium after all adjustments
  name: annual_premium
  type: number
- description: Currency code
  name: currency
  type: string
- description: List of individual rating factors applied
  name: factors
  type: array
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-rating-factors-response-schema.json
slug: api-connect-rating-factors-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-rating-factors-response-schema.json\",\n  \"title\": \"RatingFactorsResponse\",\n  \"description\": \"Detailed premium breakdown and rating factors for an estimate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the estimate\",\n      \"example\": \"est-500123\"\n    },\n    \"base_premium\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Base premium before adjustments\",\n      \"example\": 980.0\n    },\n    \"risk_loading\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Additional risk-based premium loading\",\n      \"example\": 200.0\n    },\n    \"discounts\": {\n      \"type\": \"number\",\n      \"format\"\
  : \"double\",\n      \"description\": \"Applied discounts\",\n      \"example\": 50.0\n    },\n    \"stamp_duty\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Government stamp duty\",\n      \"example\": 120.0\n    },\n    \"annual_premium\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Final annual premium after all adjustments\",\n      \"example\": 1250.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"AUD\"\n    },\n    \"factors\": {\n      \"type\": \"array\",\n      \"description\": \"List of individual rating factors applied\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RatingFactor\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-rating-factors-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: RatingFactorsResponse
---
