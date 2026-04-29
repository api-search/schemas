---
description: Use of Proceeds for a Fixed Income security.
layout: schema
name: useOfProceeds
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Use of proceeds.
  name: useOfProceeds
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-use-of-proceeds-schema.json
slug: factset-terms-and-conditions-use-of-proceeds
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"useOfProceeds\",\n  \"type\": \"object\",\n  \"description\": \"Use of Proceeds for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"useOfProceeds\": {\n      \"type\": \"string\",\n      \"description\": \"Use of proceeds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-use-of-proceeds-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: useOfProceeds
---
