---
description: The account/benchmark parameter for Vault calculation.
layout: schema
name: VaultIdentifier
properties_list:
- description: User's FactSet account path OR benchmark.
  name: id
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-vault-identifier-schema.json
slug: factset-vault-vault-identifier
source_filename: factset-vault-vault-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VaultIdentifier\",\n  \"type\": \"object\",\n  \"description\": \"The account/benchmark parameter for Vault calculation.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User's FactSet account path OR benchmark.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-vault-identifier-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: VaultIdentifier
---
