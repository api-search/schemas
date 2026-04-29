---
description: Document model
layout: schema
name: DocumentModel
properties_list:
- description: The resolved URL pointing to the location of the underlying report
  name: url
  type: string
- description: string property to denote what Product created this document.
  name: productType
  type: string
- description: The documents tags, represented in a key value format with the tag name as the key; and the tag's value as the value
  name: tags
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-analytics-datastore-document-model-schema.json
slug: factset-analytics-datastore-document-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentModel\",\n  \"type\": \"object\",\n  \"description\": \"Document model\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The resolved URL pointing to the location of the underlying report\"\n    },\n    \"productType\": {\n      \"type\": \"string\",\n      \"description\": \"string property to denote what Product created this document.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"The documents tags, represented in a key value format with the tag name as the key; and the tag's value as the value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-analytics-datastore-document-model-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DocumentModel
---
