---
description: ''
layout: schema
name: MessageCreateRequest
properties_list:
- description: The subject of the message.
  name: subject
  type: string
- description: ''
  name: toRecipients
  type: array
- description: ''
  name: ccRecipients
  type: array
- description: ''
  name: bccRecipients
  type: array
- description: ''
  name: replyTo
  type: array
- description: ''
  name: importance
  type: string
- description: ''
  name: isDeliveryReceiptRequested
  type: boolean
- description: ''
  name: isReadReceiptRequested
  type: boolean
- description: ''
  name: categories
  type: array
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-message-create-request-schema.json
slug: microsoft-graph-message-create-request
source_filename: microsoft-graph-message-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the message.\"\n    },\n    \"toRecipients\": {\n      \"type\": \"array\"\n    },\n    \"ccRecipients\": {\n      \"type\": \"array\"\n    },\n    \"bccRecipients\": {\n      \"type\": \"array\"\n    },\n    \"replyTo\": {\n      \"type\": \"array\"\n    },\n    \"importance\": {\n      \"type\": \"string\"\n    },\n    \"isDeliveryReceiptRequested\": {\n      \"type\": \"boolean\"\n    },\n    \"isReadReceiptRequested\": {\n      \"type\": \"boolean\"\n    },\n    \"categories\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-message-create-request-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: MessageCreateRequest
---
