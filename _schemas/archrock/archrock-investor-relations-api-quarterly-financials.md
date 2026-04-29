---
description: ''
layout: schema
name: QuarterlyFinancials
properties_list:
- description: ''
  name: year
  type: integer
- description: ''
  name: quarter
  type: integer
- description: Total revenue in millions USD
  name: revenue
  type: number
- description: Gross margin percentage
  name: grossMargin
  type: number
- description: Adjusted EBITDA in millions USD
  name: ebitda
  type: number
- description: Net income in millions USD
  name: netIncome
  type: number
- description: ''
  name: earningsPerShare
  type: number
- description: ''
  name: dividendPerShare
  type: number
- description: ''
  name: operatingCashFlow
  type: number
- description: ''
  name: capitalExpenditures
  type: number
- description: ''
  name: reportDate
  type: string
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-quarterly-financials-schema.json
slug: archrock-investor-relations-api-quarterly-financials
source_filename: archrock-investor-relations-api-quarterly-financials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-quarterly-financials-schema.json\",\n  \"title\": \"QuarterlyFinancials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"year\": {\n      \"type\": \"integer\"\n    },\n    \"quarter\": {\n      \"type\": \"integer\"\n    },\n    \"revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Total revenue in millions USD\"\n    },\n    \"grossMargin\": {\n      \"type\": \"number\",\n      \"description\": \"Gross margin percentage\"\n    },\n    \"ebitda\": {\n      \"type\": \"number\",\n      \"description\": \"Adjusted EBITDA in millions USD\"\n    },\n    \"netIncome\": {\n      \"type\": \"number\",\n      \"description\": \"Net income in millions USD\"\n    },\n    \"earningsPerShare\": {\n      \"type\": \"number\"\n    },\n    \"dividendPerShare\": {\n  \
  \    \"type\": \"number\"\n    },\n    \"operatingCashFlow\": {\n      \"type\": \"number\"\n    },\n    \"capitalExpenditures\": {\n      \"type\": \"number\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-quarterly-financials-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: QuarterlyFinancials
---
