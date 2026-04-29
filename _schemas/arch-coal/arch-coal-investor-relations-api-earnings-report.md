---
description: ''
layout: schema
name: EarningsReport
properties_list:
- description: Fiscal year
  name: year
  type: integer
- description: Quarter (null for annual)
  name: quarter
  type: integer
- description: Total revenue in USD
  name: revenue
  type: integer
- description: Adjusted EBITDA in USD
  name: ebitda
  type: integer
- description: Net income in USD
  name: netIncome
  type: integer
- description: Diluted earnings per share in USD
  name: earningsPerShare
  type: number
provider_name: Arch Coal
provider_slug: arch-coal
schema_file: json-schema/arch-coal-investor-relations-api-earnings-report-schema.json
slug: arch-coal-investor-relations-api-earnings-report
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Fiscal year\",\n      \"example\": 2025\n    },\n    \"quarter\": {\n      \"type\": \"integer\",\n      \"description\": \"Quarter (null for annual)\",\n      \"example\": 4\n    },\n    \"revenue\": {\n      \"type\": \"integer\",\n      \"description\": \"Total revenue in USD\",\n      \"example\": 782000000\n    },\n    \"ebitda\": {\n      \"type\": \"integer\",\n      \"description\": \"Adjusted EBITDA in USD\",\n      \"example\": 245000000\n    },\n    \"netIncome\": {\n      \"type\": \"integer\",\n      \"description\": \"Net income in USD\",\n      \"example\": 198000000\n    },\n    \"earningsPerShare\": {\n      \"type\": \"number\",\n      \"description\": \"Diluted earnings per share in USD\",\n      \"example\": 12.45\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-earnings-report-schema.json\"\
  ,\n  \"title\": \"EarningsReport\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-earnings-report-schema.json
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
title: EarningsReport
---
