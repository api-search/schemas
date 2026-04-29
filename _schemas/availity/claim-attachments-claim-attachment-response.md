---
description: ClaimAttachmentResponse schema from Availity API
layout: schema
name: ClaimAttachmentResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: controlNumber
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-attachments-claim-attachment-response-schema.json
slug: claim-attachments-claim-attachment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-attachments-claim-attachment-response-schema.json\",\n  \"title\": \"ClaimAttachmentResponse\",\n  \"description\": \"ClaimAttachmentResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUBMITTED\",\n        \"ACCEPTED\",\n        \"REJECTED\",\n        \"PENDING\"\n      ],\n      \"example\": \"ACCEPTED\"\n    },\n    \"controlNumber\": {\n      \"type\": \"string\",\n      \"example\": \"ATT-2025-001234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-attachments-claim-attachment-response-schema.json
tags: []
title: ClaimAttachmentResponse
---
