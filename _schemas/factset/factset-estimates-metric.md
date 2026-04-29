---
description: ''
layout: schema
name: metric
properties_list:
- description: Metric identifier to be used as `metrics` input in the FactSet Estimate endpoints.
  name: metric
  type: string
- description: Plain text name of the metric.
  name: name
  type: string
- description: Primary Category of metric item, such as, FINANCIAL_STATEMENT or INDUSTRY_METRIC
  name: category
  type: string
- description: Sub-category of metric items, such as the INCOME_STATEMENT or AIRLINES.
  name: subcategory
  type: string
- description: The Online Assistant Page URL, used to lookup the definition and methodology of the requested item.
  name: OAurl
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-estimates-metric-schema.json
slug: factset-estimates-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"metric\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"Metric identifier to be used as `metrics` input in the FactSet Estimate endpoints.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text name of the metric.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Category of metric item, such as, FINANCIAL_STATEMENT or INDUSTRY_METRIC\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"Sub-category of metric items, such as the INCOME_STATEMENT or AIRLINES.\"\n    },\n    \"OAurl\": {\n      \"type\": \"string\",\n      \"description\": \"The Online Assistant Page URL, used to lookup the definition and methodology of the requested item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-estimates-metric-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: metric
---
