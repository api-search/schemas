---
description: ''
layout: schema
name: VaultComponent
properties_list:
- description: Vault component identifier
  name: id
  type: string
- description: Currency iso code saved in the document
  name: currencyisocode
  type: string
- description: Snapshot
  name: snapshot
  type: boolean
- description: The path to the document
  name: path
  type: string
- description: Component name.
  name: name
  type: string
- description: Component category.
  name: category
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-vault-component-schema.json
slug: factset-vault-vault-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VaultComponent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Vault component identifier\"\n    },\n    \"currencyisocode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency iso code saved in the document\"\n    },\n    \"snapshot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Snapshot\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the document\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Component name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Component category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-vault-component-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: VaultComponent
---
