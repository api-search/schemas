---
description: Represents a file attachment on a message.
layout: schema
name: Attachment
properties_list:
- description: Unique identifier for the attachment
  name: id
  type: string
- description: MIME type of the attachment
  name: type
  type: string
- description: URL to access the attachment
  name: url
  type: string
- description: Original filename
  name: filename
  type: string
- description: File size in bytes
  name: size
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-attachment-schema.json
slug: conversations-api-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-attachment-schema.json\",\n  \"title\": \"Attachment\",\n  \"description\": \"Represents a file attachment on a message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the attachment\",\n      \"example\": \"attach_001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the attachment\",\n      \"example\": \"application/pdf\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to access the attachment\",\n      \"example\": \"https://api.hubapi.com/files/v3/files/attach_001\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename\",\n      \"example\":\
  \ \"invoice.pdf\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes\",\n      \"example\": 102400\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-attachment-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: Attachment
---
