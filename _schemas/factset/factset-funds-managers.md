---
description: ''
layout: schema
name: managers
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: Proper Name of the Fund Manager
  name: managerName
  type: string
- description: Proper Title of the Fund Manager
  name: managerTitle
  type: string
- description: Phone Number of the Fund Manager
  name: managerPhone
  type: string
- description: Inception Date of the Fund Manager
  name: managerInceptionDate
  type: string
- description: Job Identifier for the Fund Manager
  name: managerJobId
  type: integer
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-managers-schema.json
slug: factset-funds-managers
source_filename: factset-funds-managers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"managers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"managerName\": {\n      \"type\": \"string\",\n      \"description\": \"Proper Name of the Fund Manager\"\n    },\n    \"managerTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Proper Title of the Fund Manager\"\n    },\n    \"managerPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone Number of the Fund Manager\"\n    },\n    \"managerInceptionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Inception Date of the Fund Manager\"\n    },\n    \"managerJobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Job Identifier for the Fund\
  \ Manager\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-managers-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: managers
---
