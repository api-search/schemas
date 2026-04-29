---
description: ''
layout: schema
name: DataSourceInstance
properties_list:
- description: ''
  name: dstInstanceId
  type: integer
- description: ''
  name: dstInstanceType
  type: integer
- description: ''
  name: rows
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-data-source-instance-schema.json
slug: factset-vermilion-data-source-instance
source_filename: factset-vermilion-data-source-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceInstance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dstInstanceId\": {\n      \"type\": \"integer\"\n    },\n    \"dstInstanceType\": {\n      \"type\": \"integer\"\n    },\n    \"rows\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-data-source-instance-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DataSourceInstance
---
