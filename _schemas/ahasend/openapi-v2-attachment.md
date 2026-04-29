---
description: Attachment schema from AhaSend API
layout: schema
name: Attachment
properties_list:
- description: If true, data must be encoded using base64. Otherwise, data will be interpreted as UTF-8
  name: base64
  type: boolean
- description: Either plaintext or base64 encoded attachment data (depending on base64 field)
  name: data
  type: string
- description: The MIME type of the attachment
  name: content_type
  type: string
- description: The disposition of the attachment
  name: content_disposition
  type: string
- description: The Content-ID of the attachment for inline images
  name: content_id
  type: string
- description: The filename of the attachment
  name: file_name
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-attachment-schema.json
slug: openapi-v2-attachment
source_filename: openapi-v2-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-attachment-schema.json\",\n  \"title\": \"Attachment\",\n  \"description\": \"Attachment schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base64\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, data must be encoded using base64. Otherwise, data will be interpreted as UTF-8\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Either plaintext or base64 encoded attachment data (depending on base64 field)\",\n      \"example\": \"example_value\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the attachment\",\n      \"example\": \"example_value\"\n    },\n    \"content_disposition\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The disposition of the attachment\",\n      \"example\": \"example_value\"\n    },\n    \"content_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Content-ID of the attachment for inline images\",\n      \"example\": \"500123\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"description\": \"The filename of the attachment\",\n      \"example\": \"Example Name\"\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"content_type\",\n    \"file_name\"\n  ],\n  \"example\": {\n    \"base64\": true,\n    \"data\": \"iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mP8/5+hHgAHggJ/PchI7wAAAABJRU5ErkJggg==\",\n    \"content_type\": \"image/png\",\n    \"file_name\": \"pixel.png\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-attachment-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Attachment
---
