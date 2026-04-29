---
description: The pointer and parameter of the error
layout: schema
name: errorSource
properties_list:
- description: Indicates which path or URI query parameter caused the error
  name: parameter
  type: string
- description: Pointer to the associated entity in the request body
  name: pointer
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-reporting-batcher-error-source-schema.json
slug: factset-portfolio-reporting-batcher-error-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"errorSource\",\n  \"type\": \"object\",\n  \"description\": \"The pointer and parameter of the error\",\n  \"properties\": {\n    \"parameter\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates which path or URI query parameter caused the error\"\n    },\n    \"pointer\": {\n      \"type\": \"string\",\n      \"description\": \"Pointer to the associated entity in the request body\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-reporting-batcher-error-source-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: errorSource
---
