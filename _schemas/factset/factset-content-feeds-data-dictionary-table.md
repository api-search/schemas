---
description: ''
layout: schema
name: Table
properties_list:
- description: Unique identifier for the table
  name: id
  type: string
- description: Schema prefix for Standard DataFeeds
  name: dbSchema
  type: string
- description: Name of the table
  name: name
  type: string
- description: A description of the table
  name: description
  type: string
- description: Flag indicating if the user is entitled to access the data in their subscriptions
  name: entitled
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-table-schema.json
slug: factset-content-feeds-data-dictionary-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the table\"\n    },\n    \"dbSchema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema prefix for Standard DataFeeds\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the table\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the table\"\n    },\n    \"entitled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the user is entitled to access the data in their subscriptions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-table-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Table
---
