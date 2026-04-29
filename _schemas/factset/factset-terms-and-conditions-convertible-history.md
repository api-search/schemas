---
description: Convertible Details for a Fixed Income security.
layout: schema
name: convertibleHistory
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Convertible Effective Date
  name: convEffDate
  type: string
- description: Convertibles Price
  name: convPrice
  type: number
- description: Convertibles Ratio
  name: convRatio
  type: number
- description: Convertibles Underlying FactSet Permanent Identifier
  name: convUlyFsymId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-convertible-history-schema.json
slug: factset-terms-and-conditions-convertible-history
source_filename: factset-terms-and-conditions-convertible-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"convertibleHistory\",\n  \"type\": \"object\",\n  \"description\": \"Convertible Details for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"convEffDate\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Effective Date\"\n    },\n    \"convPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Convertibles Price\"\n    },\n    \"convRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Convertibles Ratio\"\n    },\n    \"convUlyFsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Convertibles Underlying FactSet Permanent Identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-convertible-history-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: convertibleHistory
---
