---
description: MessageAttachment schema from AhaSend API
layout: schema
name: MessageAttachment
properties_list:
- description: Original filename of the attachment
  name: filename
  type: string
- description: Base64 encoded attachment content
  name: content
  type: string
- description: MIME content type of the attachment
  name: content_type
  type: string
- description: Content-ID for inline attachments
  name: content_id
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-attachment-schema.json
slug: openapi-v2-message-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-attachment-schema.json\",\n  \"title\": \"MessageAttachment\",\n  \"description\": \"MessageAttachment schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename of the attachment\",\n      \"example\": \"document.pdf\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Base64 encoded attachment content\",\n      \"example\": \"example_value\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME content type of the attachment\",\n      \"example\": \"application/pdf\"\n    },\n    \"content_id\": {\n      \"type\": \"string\",\n      \"description\": \"Content-ID for inline attachments\",\n      \"nullable\": true,\n\
  \      \"example\": \"image001@example.com\"\n    }\n  },\n  \"required\": [\n    \"filename\",\n    \"content\",\n    \"content_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-attachment-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: MessageAttachment
---
