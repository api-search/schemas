---
description: ''
layout: schema
name: TemplatedPAComponentParameters
properties_list:
- description: Directory to create templated components
  name: directory
  type: string
- description: Parent template id
  name: parentTemplateId
  type: string
- description: Component description.
  name: description
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-templated-pa-component-parameters-schema.json
slug: factset-pa-engine-templated-pa-component-parameters
source_filename: factset-pa-engine-templated-pa-component-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplatedPAComponentParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"type\": \"string\",\n      \"description\": \"Directory to create templated components\"\n    },\n    \"parentTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent template id\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Component description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-templated-pa-component-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TemplatedPAComponentParameters
---
