---
description: Mandate schema from Avalara API
layout: schema
name: Mandate
properties_list:
- description: ''
  name: mandateId
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ''
  name: countryName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: supportedDocumentTypes
  type: array
- description: ''
  name: inputFormats
  type: array
- description: ''
  name: workflowId
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-mandate-schema.json
slug: e-invoicing-mandate
source_filename: e-invoicing-mandate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-mandate-schema.json\",\n  \"title\": \"Mandate\",\n  \"description\": \"Mandate schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mandateId\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"countryName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"supportedDocumentTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputFormats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"workflowId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-mandate-schema.json
tags:
- Taxes
title: Mandate
---
