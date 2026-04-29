---
description: Filings Response Object
layout: schema
name: InvestmentResearch
properties_list:
- description: Data Array Object
  name: data
  type: array
- description: Meta Object
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-filings-investment-research-schema.json
slug: factset-global-filings-investment-research
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvestmentResearch\",\n  \"type\": \"object\",\n  \"description\": \"Filings Response Object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Data Array Object\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Meta Object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-filings-investment-research-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: InvestmentResearch
---
