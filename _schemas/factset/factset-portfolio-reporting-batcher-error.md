---
description: Full details of any error
layout: schema
name: error
properties_list:
- description: The error code
  name: code
  type: string
- description: Explanation specific to the occurrence of the error
  name: detail
  type: string
- description: Identifier for the error
  name: id
  type: string
- description: The title of the error
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-reporting-batcher-error-schema.json
slug: factset-portfolio-reporting-batcher-error
source_filename: factset-portfolio-reporting-batcher-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"error\",\n  \"type\": \"object\",\n  \"description\": \"Full details of any error\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Explanation specific to the occurrence of the error\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-reporting-batcher-error-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: error
---
