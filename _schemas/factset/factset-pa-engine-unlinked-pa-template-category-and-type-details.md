---
description: ''
layout: schema
name: UnlinkedPATemplateCategoryAndTypeDetails
properties_list:
- description: Type Id
  name: id
  type: string
- description: List of default columns
  name: columns
  type: array
- description: List of default groupings
  name: groups
  type: array
- description: Snapshot
  name: snapshot
  type: boolean
- description: Unlinked template category
  name: category
  type: string
- description: Unlinked template type
  name: name
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-unlinked-pa-template-category-and-type-details-schema.json
slug: factset-pa-engine-unlinked-pa-template-category-and-type-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnlinkedPATemplateCategoryAndTypeDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Type Id\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of default columns\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"List of default groupings\"\n    },\n    \"snapshot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Snapshot\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Unlinked template category\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unlinked template type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-unlinked-pa-template-category-and-type-details-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UnlinkedPATemplateCategoryAndTypeDetails
---
