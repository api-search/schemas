---
description: Covenant Detail for a Fixed Income security.
layout: schema
name: covenantDetail
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Covenant Type
  name: finCovType
  type: string
- description: Description
  name: finCovDesc
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-covenant-detail-schema.json
slug: factset-terms-and-conditions-covenant-detail
source_filename: factset-terms-and-conditions-covenant-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"covenantDetail\",\n  \"type\": \"object\",\n  \"description\": \"Covenant Detail for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"finCovType\": {\n      \"type\": \"string\",\n      \"description\": \"Covenant Type\"\n    },\n    \"finCovDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-covenant-detail-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: covenantDetail
---
