---
description: ''
layout: schema
name: TemplateContentTypes
properties_list:
- description: Template mandatory fields
  name: mandatory
  type: array
- description: Template optional fields
  name: optional
  type: array
- description: Template locked fields
  name: locked
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-template-content-types-schema.json
slug: factset-pa-engine-template-content-types
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplateContentTypes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mandatory\": {\n      \"type\": \"array\",\n      \"description\": \"Template mandatory fields\"\n    },\n    \"optional\": {\n      \"type\": \"array\",\n      \"description\": \"Template optional fields\"\n    },\n    \"locked\": {\n      \"type\": \"array\",\n      \"description\": \"Template locked fields\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-template-content-types-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TemplateContentTypes
---
