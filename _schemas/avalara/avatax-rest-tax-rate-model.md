---
description: TaxRateModel schema from Avalara API
layout: schema
name: TaxRateModel
properties_list:
- description: Total combined tax rate
  name: totalRate
  type: number
- description: ''
  name: rates
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-tax-rate-model-schema.json
slug: avatax-rest-tax-rate-model
source_filename: avatax-rest-tax-rate-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-rate-model-schema.json\",\n  \"title\": \"TaxRateModel\",\n  \"description\": \"TaxRateModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total combined tax rate\"\n    },\n    \"rates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rate\": {\n            \"type\": \"number\",\n            \"format\": \"double\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Country\",\n              \"State\",\n              \"County\",\n              \"City\",\n   \
  \           \"Special\"\n            ]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-tax-rate-model-schema.json
tags:
- Taxes
title: TaxRateModel
---
