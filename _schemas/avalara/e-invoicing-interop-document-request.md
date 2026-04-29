---
description: InteropDocumentRequest schema from Avalara API
layout: schema
name: InteropDocumentRequest
properties_list:
- description: ''
  name: dataFormat
  type: string
- description: ''
  name: data
  type: string
- description: Recipient identifier on the interop network
  name: recipientIdentifier
  type: string
- description: Identifier scheme (e.g., peppol)
  name: recipientIdentifierScheme
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-interop-document-request-schema.json
slug: e-invoicing-interop-document-request
source_filename: e-invoicing-interop-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-interop-document-request-schema.json\",\n  \"title\": \"InteropDocumentRequest\",\n  \"description\": \"InteropDocumentRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"dataFormat\",\n    \"data\",\n    \"recipientIdentifier\"\n  ],\n  \"properties\": {\n    \"dataFormat\": {\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"type\": \"string\"\n    },\n    \"recipientIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient identifier on the interop network\"\n    },\n    \"recipientIdentifierScheme\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier scheme (e.g., peppol)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-interop-document-request-schema.json
tags:
- Taxes
title: InteropDocumentRequest
---
