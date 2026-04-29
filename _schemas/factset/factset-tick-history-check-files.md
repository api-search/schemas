---
description: check-files
layout: schema
name: checkFiles
properties_list:
- description: a unique identification for the query requested
  name: id
  type: string
- description: The status of the query
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-check-files-schema.json
slug: factset-tick-history-check-files
source_filename: factset-tick-history-check-files-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"checkFiles\",\n  \"type\": \"object\",\n  \"description\": \"check-files\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"a unique identification for the query requested\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the query\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-check-files-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: checkFiles
---
