---
description: Specifies the fields in the error message
layout: schema
name: errorExample
properties_list:
- description: It specifies the unique code
  name: code
  type: string
- description: Specifies the error message
  name: title
  type: string
- description: Specifies the id
  name: id
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-error-example-schema.json
slug: factset-tick-history-error-example
source_filename: factset-tick-history-error-example-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"errorExample\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the fields in the error message\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"It specifies the unique code\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \" Specifies the error message\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the id\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-error-example-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: errorExample
---
