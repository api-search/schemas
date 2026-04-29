---
description: A file attachment.
layout: schema
name: Attachment
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: file_name
  type: string
- description: ''
  name: content_url
  type: string
- description: ''
  name: content_type
  type: string
- description: The size of the file in bytes.
  name: size
  type: integer
- description: ''
  name: thumbnails
  type: array
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-attachment-schema.json
slug: zendesk-support-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Attachment\",\n  \"type\": \"object\",\n  \"description\": \"A file attachment.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"file_name\": {\n      \"type\": \"string\"\n    },\n    \"content_url\": {\n      \"type\": \"string\"\n    },\n    \"content_type\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the file in bytes.\"\n    },\n    \"thumbnails\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-attachment-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: Attachment
---
