---
description: ''
layout: schema
name: AccountDirectories
properties_list:
- description: List of account and composite files.
  name: accounts
  type: array
- description: List of directories.
  name: directories
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-optimizer-account-directories-schema.json
slug: factset-portfolio-optimizer-account-directories
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountDirectories\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of account and composite files.\"\n    },\n    \"directories\": {\n      \"type\": \"array\",\n      \"description\": \"List of directories.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-optimizer-account-directories-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: AccountDirectories
---
