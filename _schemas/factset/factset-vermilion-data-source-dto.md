---
description: ''
layout: schema
name: DataSourceDTO
properties_list:
- description: ''
  name: dataSourceId
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: dsType
  type: string
- description: ''
  name: entities
  type: array
- description: ''
  name: outputRecordSet
  type: string
- description: ''
  name: releaseTag
  type: string
- description: ''
  name: defaultDataSourceName
  type: string
- description: ''
  name: dataPreview
  type: string
- description: ''
  name: lastUpdatedBy
  type: string
- description: ''
  name: lastUpdated
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-data-source-dto-schema.json
slug: factset-vermilion-data-source-dto
source_filename: factset-vermilion-data-source-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceDTO\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSourceId\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"dsType\": {\n      \"type\": \"string\"\n    },\n    \"entities\": {\n      \"type\": \"array\"\n    },\n    \"outputRecordSet\": {\n      \"type\": \"string\"\n    },\n    \"releaseTag\": {\n      \"type\": \"string\"\n    },\n    \"defaultDataSourceName\": {\n      \"type\": \"string\"\n    },\n    \"dataPreview\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-data-source-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DataSourceDTO
---
