---
description: ''
layout: schema
name: MessageUpdateRequest
properties_list:
- description: ''
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
  name: importance
  type: string
- description: ''
  name: isRead
  type: boolean
- description: ''
  name: categories
  type: array
- description: ''
  name: inferenceClassification
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-message-update-request-schema.json
slug: microsoft-graph-message-update-request
source_filename: microsoft-graph-message-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"toRecipients\": {\n      \"type\": \"array\"\n    },\n    \"ccRecipients\": {\n      \"type\": \"array\"\n    },\n    \"bccRecipients\": {\n      \"type\": \"array\"\n    },\n    \"importance\": {\n      \"type\": \"string\"\n    },\n    \"isRead\": {\n      \"type\": \"boolean\"\n    },\n    \"categories\": {\n      \"type\": \"array\"\n    },\n    \"inferenceClassification\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-message-update-request-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: MessageUpdateRequest
---
