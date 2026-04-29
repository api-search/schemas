---
description: Convertible Triggers for a Fixed Income security.
layout: schema
name: convertibleTriggers
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Convertible Trigger Event
  name: convTriggerEvent
  type: string
- description: Convertible Trigger Event Description
  name: convTriggerEventDesc
  type: string
- description: Convertible Trigger Id
  name: triggerId
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-convertible-triggers-schema.json
slug: factset-terms-and-conditions-convertible-triggers
source_filename: factset-terms-and-conditions-convertible-triggers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"convertibleTriggers\",\n  \"type\": \"object\",\n  \"description\": \"Convertible Triggers for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"convTriggerEvent\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Trigger Event\"\n    },\n    \"convTriggerEventDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Trigger Event Description\"\n    },\n    \"triggerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Convertible Trigger Id\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-convertible-triggers-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: convertibleTriggers
---
