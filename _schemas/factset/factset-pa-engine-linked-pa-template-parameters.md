---
description: ''
layout: schema
name: LinkedPATemplateParameters
properties_list:
- description: The directory to create a linked PA template
  name: directory
  type: string
- description: Parent component id
  name: parentComponentId
  type: string
- description: Template description
  name: description
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-linked-pa-template-parameters-schema.json
slug: factset-pa-engine-linked-pa-template-parameters
source_filename: factset-pa-engine-linked-pa-template-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinkedPATemplateParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"type\": \"string\",\n      \"description\": \"The directory to create a linked PA template\"\n    },\n    \"parentComponentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent component id\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-linked-pa-template-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: LinkedPATemplateParameters
---
