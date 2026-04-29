---
description: ''
layout: schema
name: Calculation
properties_list:
- description: The python script that will be executed
  name: script
  type: string
- description: Notebook file to be executed. Only notebooks in the Client directory are currently supported.
  name: notebook
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-programmatic-environment-calculation-schema.json
slug: factset-programmatic-environment-calculation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Calculation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"script\": {\n      \"type\": \"string\",\n      \"description\": \"The python script that will be executed\"\n    },\n    \"notebook\": {\n      \"type\": \"string\",\n      \"description\": \"Notebook file to be executed. Only notebooks in the Client directory are currently supported.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-programmatic-environment-calculation-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Calculation
---
