---
description: SubmitDocumentRequest schema from Avalara API
layout: schema
name: SubmitDocumentRequest
properties_list:
- description: Format of the e-invoice document
  name: dataFormat
  type: string
- description: Version of the data format
  name: dataFormatVersion
  type: string
- description: Base64-encoded document content or raw UBL/CII XML
  name: data
  type: string
- description: ''
  name: metadata
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-submit-document-request-schema.json
slug: e-invoicing-submit-document-request
source_filename: e-invoicing-submit-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-submit-document-request-schema.json\",\n  \"title\": \"SubmitDocumentRequest\",\n  \"description\": \"SubmitDocumentRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"dataFormat\",\n    \"data\"\n  ],\n  \"properties\": {\n    \"dataFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ubl-invoice\",\n        \"ubl-creditnote\",\n        \"cii\"\n      ],\n      \"description\": \"Format of the e-invoice document\"\n    },\n    \"dataFormatVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the data format\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded document content or raw UBL/CII XML\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n\
  \        \"workflowId\": {\n          \"type\": \"string\",\n          \"description\": \"Workflow identifier for the mandate\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\"\n        },\n        \"countryMandate\": {\n          \"type\": \"string\",\n          \"description\": \"Country mandate identifier\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-submit-document-request-schema.json
tags:
- Taxes
title: SubmitDocumentRequest
---
