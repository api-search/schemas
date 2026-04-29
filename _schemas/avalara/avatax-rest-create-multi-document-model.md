---
description: CreateMultiDocumentModel schema from Avalara API
layout: schema
name: CreateMultiDocumentModel
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-create-multi-document-model-schema.json
slug: avatax-rest-create-multi-document-model
source_filename: avatax-rest-create-multi-document-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-create-multi-document-model-schema.json\",\n  \"title\": \"CreateMultiDocumentModel\",\n  \"description\": \"CreateMultiDocumentModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MultiDocumentLineItemModel\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-create-multi-document-model-schema.json
tags:
- Taxes
title: CreateMultiDocumentModel
---
