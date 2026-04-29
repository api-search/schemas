---
description: ''
layout: schema
name: response_details
properties_list:
- description: Type of Asset Class
  name: index
  type: string
- description: Symbol is the only value that should be passed back to any FactSet services to retrieve data
  name: symbol
  type: string
- description: Name of the related entity
  name: name
  type: string
- description: Displays Entity ID's for public companies and only if the asset class is equities
  name: entity_id
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-id-lookup-response_details-schema.json
slug: factset-id-lookup-response_details
source_filename: factset-id-lookup-response_details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"response_details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Type of Asset Class\"\n    },\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Symbol is the only value that should be passed back to any FactSet services to retrieve data\\n\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the related entity\"\n    },\n    \"entity_id\": {\n      \"type\": \"string\",\n      \"description\": \"Displays Entity ID's for public companies and only if the asset class is equities\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-id-lookup-response_details-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: response_details
---
