---
description: A single business or geographic segment data point for a company.
layout: schema
name: Segment
properties_list:
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: FactSet Regional Security Identifier.
  name: fsymId
  type: '[''string'', ''null'']'
- description: The segment metric (SALES, OPINC, ASSETS, DEP, CAPEX).
  name: metric
  type: '[''string'', ''null'']'
- description: Report labels of the segment type requested.
  name: label
  type: '[''string'', ''null'']'
- description: Date for the period requested in YYYY-MM-DD format.
  name: date
  type: '[''string'', ''null'']'
- description: Segment metric value. May be a number or string.
  name: value
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-segment-schema.json
slug: factset-fundamentals-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Segment\",\n  \"type\": \"object\",\n  \"description\": \"A single business or geographic segment data point for a company.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"FactSet Regional Security Identifier.\"\n    },\n    \"metric\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The segment metric (SALES, OPINC, ASSETS, DEP, CAPEX).\"\n    },\n    \"label\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Report labels of the segment type requested.\"\n    },\n    \"date\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date for the period requested in YYYY-MM-DD format.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Segment metric value. May be a number or string.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-segment-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Segment
---
