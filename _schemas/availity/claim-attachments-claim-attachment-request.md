---
description: ClaimAttachmentRequest schema from Availity API
layout: schema
name: ClaimAttachmentRequest
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: claimNumber
  type: string
- description: ''
  name: provider
  type: object
- description: ''
  name: attachmentType
  type: string
- description: ''
  name: attachments
  type: array
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-attachments-claim-attachment-request-schema.json
slug: claim-attachments-claim-attachment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-attachments-claim-attachment-request-schema.json\",\n  \"title\": \"ClaimAttachmentRequest\",\n  \"description\": \"ClaimAttachmentRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"claimNumber\",\n    \"provider\",\n    \"attachments\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"claimNumber\": {\n      \"type\": \"string\",\n      \"example\": \"CLM-2025-001234\"\n    },\n    \"provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"npi\": {\n          \"type\": \"string\",\n          \"example\": \"1234567890\"\n        }\n      }\n    },\n    \"attachmentType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STRUCTURED\",\n        \"\
  UNSTRUCTURED\"\n      ],\n      \"example\": \"UNSTRUCTURED\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"contentType\": {\n            \"type\": \"string\",\n            \"example\": \"application/pdf\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Operative Report\"\n          },\n          \"data\": {\n            \"type\": \"string\",\n            \"format\": \"byte\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-attachments-claim-attachment-request-schema.json
tags: []
title: ClaimAttachmentRequest
---
