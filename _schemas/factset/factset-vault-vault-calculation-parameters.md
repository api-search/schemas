---
description: ''
layout: schema
name: VaultCalculationParameters
properties_list:
- description: The Vault component identifier to analyze.
  name: componentid
  type: string
- description: Vault Configuration identifier.
  name: configid
  type: string
- description: Component detail type for the Vault component. It can be GROUPS or GROUPSALL or TOTALS or SECURITIES.
  name: componentdetail
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-vault-calculation-parameters-schema.json
slug: factset-vault-vault-calculation-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VaultCalculationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentid\": {\n      \"type\": \"string\",\n      \"description\": \"The Vault component identifier to analyze.\"\n    },\n    \"configid\": {\n      \"type\": \"string\",\n      \"description\": \"Vault Configuration identifier.\"\n    },\n    \"componentdetail\": {\n      \"type\": \"string\",\n      \"description\": \"Component detail type for the Vault component. It can be GROUPS or GROUPSALL or TOTALS or SECURITIES.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-vault-calculation-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: VaultCalculationParameters
---
