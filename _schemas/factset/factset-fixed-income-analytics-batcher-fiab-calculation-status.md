---
description: ''
layout: schema
name: FIABCalculationStatus
properties_list:
- description: ''
  name: id
  type: string
- description: FIAB service batch status integer definitions. See https://pages.github.factset.com/FactSet/fipa-inf-docs/service/fiab_batch_api.html#lt-uuid-gt.
  name: status
  type: string
- description: ''
  name: startdatetime
  type: string
- description: ''
  name: completiondatetime
  type: string
- description: ''
  name: progress
  type: integer
- description: ''
  name: batchevents
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-status-schema.json
slug: factset-fixed-income-analytics-batcher-fiab-calculation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FIABCalculationStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"FIAB service batch status integer definitions.  See https://pages.github.factset.com/FactSet/fipa-inf-docs/service/fiab_batch_api.html#lt-uuid-gt.\"\n    },\n    \"startdatetime\": {\n      \"type\": \"string\"\n    },\n    \"completiondatetime\": {\n      \"type\": \"string\"\n    },\n    \"progress\": {\n      \"type\": \"integer\"\n    },\n    \"batchevents\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: FIABCalculationStatus
---
