---
description: ''
layout: schema
name: LinkedPATemplate
properties_list:
- description: Template directory.
  name: directory
  type: string
- description: snapshot.
  name: snapshot
  type: boolean
- description: Template id.
  name: id
  type: string
- description: Template description.
  name: description
  type: string
- description: Template name.
  name: name
  type: string
- description: Template parent tile.
  name: parentComponentId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-linked-pa-template-schema.json
slug: factset-pa-engine-linked-pa-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinkedPATemplate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"type\": \"string\",\n      \"description\": \"Template directory.\"\n    },\n    \"snapshot\": {\n      \"type\": \"boolean\",\n      \"description\": \"snapshot.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Template id.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name.\"\n    },\n    \"parentComponentId\": {\n      \"type\": \"string\",\n      \"description\": \"Template parent tile.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-linked-pa-template-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: LinkedPATemplate
---
