---
description: LodgingTaxRateResponse schema from Avalara API
layout: schema
name: LodgingTaxRateResponse
properties_list:
- description: Total combined lodging tax rate
  name: totalRate
  type: number
- description: ''
  name: rates
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/mylodgetax-lodging-tax-rate-response-schema.json
slug: mylodgetax-lodging-tax-rate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-lodging-tax-rate-response-schema.json\",\n  \"title\": \"LodgingTaxRateResponse\",\n  \"description\": \"LodgingTaxRateResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total combined lodging tax rate\"\n    },\n    \"rates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"jurisdiction\": {\n            \"type\": \"string\"\n          },\n          \"jurisdictionType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"State\",\n              \"County\",\n              \"City\",\n              \"District\"\n            ]\n          },\n          \"taxName\": {\n\
  \            \"type\": \"string\"\n          },\n          \"rate\": {\n            \"type\": \"number\",\n            \"format\": \"double\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-lodging-tax-rate-response-schema.json
tags:
- Taxes
title: LodgingTaxRateResponse
---
