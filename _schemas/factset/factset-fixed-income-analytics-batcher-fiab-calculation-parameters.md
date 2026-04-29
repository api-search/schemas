---
description: ''
layout: schema
name: FIABCalculationParameters
properties_list:
- description: FiabDocument (optional) - FIAB document to use as a template. Should be a path to a FIAB document. Expects a GUI-style path (Client:/foo/bar)
  name: fiabdocument
  type: string
- description: Master Security List. Analytics results will be written to the selected MSL. Expects a GUI-style path (Client:/foo/bar)
  name: msl
  type: string
- description: FISettingsDocument (optional) - The given @FIS document will be used to configure analytics assumptions and settings. Expects a GUI-style path (Client:/foo/bar)
  name: fisettingsdocument
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-parameters-schema.json
slug: factset-fixed-income-analytics-batcher-fiab-calculation-parameters
source_filename: factset-fixed-income-analytics-batcher-fiab-calculation-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FIABCalculationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fiabdocument\": {\n      \"type\": \"string\",\n      \"description\": \"FiabDocument (optional) - FIAB document to use as a template. Should\\r\\nbe a path to a FIAB document. Expects a GUI-style path (Client:/foo/bar)\"\n    },\n    \"msl\": {\n      \"type\": \"string\",\n      \"description\": \"Master Security List. Analytics results will be written to the selected MSL. Expects a GUI-style path (Client:/foo/bar)\"\n    },\n    \"fisettingsdocument\": {\n      \"type\": \"string\",\n      \"description\": \"FISettingsDocument (optional) - The given @FIS document will be used to\\r\\nconfigure analytics assumptions and settings. Expects a GUI-style path (Client:/foo/bar)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fixed-income-analytics-batcher-fiab-calculation-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: FIABCalculationParameters
---
