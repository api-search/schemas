---
description: Risk factor exposure for a portfolio
layout: schema
name: FactorExposure
properties_list:
- description: Risk factor name
  name: factorName
  type: string
- description: Factor exposure value
  name: exposure
  type: number
- description: Contribution to portfolio risk
  name: contribution
  type: number
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-factor-exposure-schema.json
slug: aladdin-studio-graph-factor-exposure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-factor-exposure-schema.json\",\n  \"title\": \"FactorExposure\",\n  \"description\": \"Risk factor exposure for a portfolio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"factorName\": {\n      \"type\": \"string\",\n      \"description\": \"Risk factor name\",\n      \"example\": \"Market\"\n    },\n    \"exposure\": {\n      \"type\": \"number\",\n      \"description\": \"Factor exposure value\",\n      \"example\": 1.02\n    },\n    \"contribution\": {\n      \"type\": \"number\",\n      \"description\": \"Contribution to portfolio risk\",\n      \"example\": 0.0285\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-factor-exposure-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: FactorExposure
---
