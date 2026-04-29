---
description: ''
layout: schema
name: DateParametersSummary
properties_list:
- description: Start date in YYYYMMDD format.
  name: startdate
  type: string
- description: End date in YYYYMMDD format.
  name: enddate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-date-parameters-summary-schema.json
slug: factset-vault-date-parameters-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DateParametersSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startdate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date in YYYYMMDD format.\"\n    },\n    \"enddate\": {\n      \"type\": \"string\",\n      \"description\": \"End date in YYYYMMDD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-date-parameters-summary-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DateParametersSummary
---
