---
description: ''
layout: schema
name: PAPricingSource
properties_list:
- description: Pricing source Name
  name: name
  type: string
- description: Pricing source directory
  name: directory
  type: string
- description: Pricing source category
  name: category
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-pa-pricing-source-schema.json
slug: factset-pa-engine-pa-pricing-source
source_filename: factset-pa-engine-pa-pricing-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PAPricingSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing source Name\"\n    },\n    \"directory\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing source directory\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing source category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-pricing-source-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PAPricingSource
---
