---
description: ''
layout: schema
name: ModelImportRequest
properties_list:
- description: Model name
  name: name
  type: string
- description: AMEFF XML or JSON model content
  name: content
  type: string
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-model-import-request-schema.json
slug: archimate-model-exchange-api-model-import-request
source_filename: archimate-model-exchange-api-model-import-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model name\",\n      \"example\": \"Imported Architecture Model\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"AMEFF XML or JSON model content\",\n      \"example\": \"<model>...</model>\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-import-request-schema.json\",\n  \"title\": \"ModelImportRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-import-request-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: ModelImportRequest
---
