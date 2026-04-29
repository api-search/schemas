---
description: ''
layout: schema
name: FIABCalculationStatusSummary
properties_list:
- description: Request time of calculation.
  name: requesttime
  type: string
- description: Last poll time of calculation.
  name: lastpolltime
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-status-summary-schema.json
slug: factset-fixed-income-analytics-batcher-fiab-calculation-status-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FIABCalculationStatusSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requesttime\": {\n      \"type\": \"string\",\n      \"description\": \"Request time of calculation.\"\n    },\n    \"lastpolltime\": {\n      \"type\": \"string\",\n      \"description\": \"Last poll time of calculation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-status-summary-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: FIABCalculationStatusSummary
---
