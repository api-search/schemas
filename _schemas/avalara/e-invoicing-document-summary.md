---
description: DocumentSummary schema from Avalara API
layout: schema
name: DocumentSummary
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: documentType
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: senderName
  type: string
- description: ''
  name: recipientName
  type: string
- description: ''
  name: submissionDate
  type: string
- description: ''
  name: countryCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-summary-schema.json
slug: e-invoicing-document-summary
source_filename: e-invoicing-document-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-summary-schema.json\",\n  \"title\": \"DocumentSummary\",\n  \"description\": \"DocumentSummary schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"documentType\": {\n      \"type\": \"string\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"senderName\": {\n      \"type\": \"string\"\n    },\n    \"recipientName\": {\n      \"type\": \"string\"\n    },\n    \"submissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-summary-schema.json
tags:
- Taxes
title: DocumentSummary
---
