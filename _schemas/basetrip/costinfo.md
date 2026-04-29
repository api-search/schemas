---
description: ''
layout: schema
name: CostInfo
properties_list:
- description: ''
  name: country
  type: string
- description: ''
  name: currency
  type: string
- description: Budget traveler daily cost in USD
  name: budgetPerDay
  type: number
- description: Mid-range daily cost in USD
  name: midRangePerDay
  type: number
- description: Luxury daily cost in USD
  name: luxuryPerDay
  type: number
- description: ''
  name: categories
  type: object
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/costinfo.json
slug: costinfo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/costinfo.json\",\n  \"title\": \"CostInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"budgetPerDay\": {\n      \"type\": \"number\",\n      \"description\": \"Budget traveler daily cost in USD\"\n    },\n    \"midRangePerDay\": {\n      \"type\": \"number\",\n      \"description\": \"Mid-range daily cost in USD\"\n    },\n    \"luxuryPerDay\": {\n      \"type\": \"number\",\n      \"description\": \"Luxury daily cost in USD\"\n    },\n    \"categories\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"accommodation\": {\n          \"type\": \"number\"\n        },\n        \"food\": {\n          \"type\": \"number\"\n        },\n        \"transport\": {\n          \"type\"\
  : \"number\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/costinfo.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: CostInfo
---
