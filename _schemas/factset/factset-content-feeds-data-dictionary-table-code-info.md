---
description: ''
layout: schema
name: TableCodeInfo
properties_list:
- description: Flag indicating if the field is represented as a code in Standard DataFeeds
  name: dataItemIsCode
  type: boolean
- description: Unique identifier for the code
  name: codeFieldId
  type: string
- description: String value for the code as it appears in Standard DataFeeds
  name: codeString
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-table-code-info-schema.json
slug: factset-content-feeds-data-dictionary-table-code-info
source_filename: factset-content-feeds-data-dictionary-table-code-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCodeInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataItemIsCode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the field is represented as a code in Standard DataFeeds\"\n    },\n    \"codeFieldId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the code\"\n    },\n    \"codeString\": {\n      \"type\": \"string\",\n      \"description\": \"String value for the code as it appears in Standard DataFeeds\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-table-code-info-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TableCodeInfo
---
