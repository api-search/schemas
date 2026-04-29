---
description: ''
layout: schema
name: VaultConfiguration
properties_list:
- description: Configuration name.
  name: name
  type: string
- description: ''
  name: accounts
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-vault-configuration-schema.json
slug: factset-vault-vault-configuration
source_filename: factset-vault-vault-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VaultConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name.\"\n    },\n    \"accounts\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-vault-configuration-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: VaultConfiguration
---
