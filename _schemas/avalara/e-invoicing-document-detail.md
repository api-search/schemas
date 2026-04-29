---
description: DocumentDetail schema from Avalara API
layout: schema
name: DocumentDetail
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: dataFormat
  type: string
- description: ''
  name: documentType
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: sender
  type: object
- description: ''
  name: recipient
  type: object
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: submissionDate
  type: string
- description: ''
  name: events
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-detail-schema.json
slug: e-invoicing-document-detail
source_filename: e-invoicing-document-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-detail-schema.json\",\n  \"title\": \"DocumentDetail\",\n  \"description\": \"DocumentDetail schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"dataFormat\": {\n      \"type\": \"string\"\n    },\n    \"documentType\": {\n      \"type\": \"string\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/components/schemas/Party\"\n    },\n    \"recipient\": {\n      \"$ref\": \"#/components/schemas/Party\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currencyCode\"\
  : {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"submissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DocumentEvent\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-detail-schema.json
tags:
- Taxes
title: DocumentDetail
---
