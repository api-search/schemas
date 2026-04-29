---
description: Error Example Object
layout: schema
name: ErrorExample
properties_list:
- description: Specifies the error code.
  name: code
  type: string
- description: Specifies the error message.
  name: title
  type: string
- description: Specifies the id.
  name: id
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-filings-error-example-schema.json
slug: factset-global-filings-error-example
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorExample\",\n  \"type\": \"object\",\n  \"description\": \"Error Example Object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the error code.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \" Specifies the error message.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the id.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-filings-error-example-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ErrorExample
---
