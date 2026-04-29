---
description: ''
layout: schema
name: UnlinkedPATemplateUpdateParameters
properties_list:
- description: Template description
  name: description
  type: string
- description: List of accounts
  name: accounts
  type: array
- description: List of benchmarks
  name: benchmarks
  type: array
- description: List of columns for the PA calculation
  name: columns
  type: array
- description: List of groupings for the PA calculation
  name: groups
  type: array
- description: Currency ISO code for calculation.
  name: currencyisocode
  type: string
- description: PA storage type. It can be GROUPS or GROUPSALL or TOTALS or SECURITIES.
  name: componentdetail
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-unlinked-pa-template-update-parameters-schema.json
slug: factset-pa-engine-unlinked-pa-template-update-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnlinkedPATemplateUpdateParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts\"\n    },\n    \"benchmarks\": {\n      \"type\": \"array\",\n      \"description\": \"List of benchmarks\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of columns for the PA calculation\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"List of groupings for the PA calculation\"\n    },\n    \"currencyisocode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code for calculation.\"\n    },\n    \"componentdetail\": {\n      \"type\": \"string\",\n      \"description\": \"PA storage type. It can be GROUPS or GROUPSALL\
  \ or TOTALS or SECURITIES.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-unlinked-pa-template-update-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UnlinkedPATemplateUpdateParameters
---
