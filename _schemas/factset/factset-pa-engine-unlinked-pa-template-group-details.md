---
description: ''
layout: schema
name: UnlinkedPATemplateGroupDetails
properties_list:
- description: Unlinked template group name
  name: name
  type: string
- description: FactSet-defined or User-defined Group identifier.
  name: id
  type: string
- description: Grouping frequency
  name: frequency
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-unlinked-pa-template-group-details-schema.json
slug: factset-pa-engine-unlinked-pa-template-group-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnlinkedPATemplateGroupDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unlinked template group name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet-defined or User-defined Group identifier.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Grouping frequency\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-unlinked-pa-template-group-details-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UnlinkedPATemplateGroupDetails
---
