---
description: ''
layout: schema
name: ComponentSummary
properties_list:
- description: Component name.
  name: name
  type: string
- description: Component category.
  name: category
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-component-summary-schema.json
slug: factset-vault-component-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComponentSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Component name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Component category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-component-summary-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ComponentSummary
---
