---
description: ''
layout: schema
name: RateResponse
properties_list:
- description: Quote reference number
  name: quoteNumber
  type: string
- description: Total freight charge in USD
  name: totalCharge
  type: number
- description: Estimated transit days
  name: transitDays
  type: integer
- description: Service level
  name: serviceLevel
  type: string
- description: Quote expiration timestamp
  name: expiresAt
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-rate-response-schema.json
slug: arcbest-api-rate-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"quoteNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Quote reference number\",\n      \"example\": \"Q-20260419-001\"\n    },\n    \"totalCharge\": {\n      \"type\": \"number\",\n      \"description\": \"Total freight charge in USD\",\n      \"example\": 425.5\n    },\n    \"transitDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated transit days\",\n      \"example\": 3\n    },\n    \"serviceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Service level\",\n      \"example\": \"STANDARD\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Quote expiration timestamp\",\n      \"example\": \"2026-04-26T23:59:59Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-rate-response-schema.json\"\
  ,\n  \"title\": \"RateResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-rate-response-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: RateResponse
---
