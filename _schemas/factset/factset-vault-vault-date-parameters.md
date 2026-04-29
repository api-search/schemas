---
description: The date parameters for Vault calculation
layout: schema
name: VaultDateParameters
properties_list:
- description: Calculation's start date.
  name: startdate
  type: string
- description: Calculation's end date.
  name: enddate
  type: string
- description: Calculation's frequency.
  name: frequency
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-vault-date-parameters-schema.json
slug: factset-vault-vault-date-parameters
source_filename: factset-vault-vault-date-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VaultDateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The date parameters for Vault calculation\",\n  \"properties\": {\n    \"startdate\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's start date.\"\n    },\n    \"enddate\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's end date.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's frequency.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-vault-date-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: VaultDateParameters
---
