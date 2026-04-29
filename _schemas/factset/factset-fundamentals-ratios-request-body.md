---
description: Request parameters for financial ratio data.
layout: schema
name: RatiosRequestBody
properties_list:
- description: Ratio subcategory filter.
  name: subcategory
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-ratios-request-body-schema.json
slug: factset-fundamentals-ratios-request-body
source_filename: factset-fundamentals-ratios-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RatiosRequestBody\",\n  \"type\": \"object\",\n  \"description\": \"Request parameters for financial ratio data.\",\n  \"properties\": {\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"Ratio subcategory filter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-ratios-request-body-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: RatiosRequestBody
---
