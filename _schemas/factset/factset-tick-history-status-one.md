---
description: request-files
layout: schema
name: StatusOne
properties_list:
- description: a unique identification for the query requested
  name: id
  type: string
- description: The status of the query
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-status-one-schema.json
slug: factset-tick-history-status-one
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatusOne\",\n  \"type\": \"object\",\n  \"description\": \"request-files\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"a unique identification for the query requested\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the query\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-status-one-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: StatusOne
---
