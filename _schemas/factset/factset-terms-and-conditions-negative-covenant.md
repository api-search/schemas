---
description: Negative Covenant for a Fixed Income security.
layout: schema
name: negativeCovenant
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Negative Covenant Level
  name: negCovenantLvl
  type: string
- description: Negative Covenant Type
  name: negCovenantType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-negative-covenant-schema.json
slug: factset-terms-and-conditions-negative-covenant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"negativeCovenant\",\n  \"type\": \"object\",\n  \"description\": \"Negative Covenant for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"negCovenantLvl\": {\n      \"type\": \"string\",\n      \"description\": \"Negative Covenant Level\"\n    },\n    \"negCovenantType\": {\n      \"type\": \"string\",\n      \"description\": \"Negative Covenant Type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-negative-covenant-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: negativeCovenant
---
