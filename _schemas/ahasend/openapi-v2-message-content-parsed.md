---
description: MessageContentParsed schema from AhaSend API
layout: schema
name: MessageContentParsed
properties_list:
- description: Array of message content parts (text, HTML, etc.)
  name: parts
  type: array
- description: Array of message attachments
  name: attachments
  type: array
- description: Email headers as key-value pairs (values are arrays to handle multiple headers with same name)
  name: headers
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-content-parsed-schema.json
slug: openapi-v2-message-content-parsed
source_filename: openapi-v2-message-content-parsed-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-content-parsed-schema.json\",\n  \"title\": \"MessageContentParsed\",\n  \"description\": \"MessageContentParsed schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MessageContentPart\"\n      },\n      \"description\": \"Array of message content parts (text, HTML, etc.)\",\n      \"example\": [\n        {\n          \"content_type\": \"example_value\",\n          \"content\": \"example_value\"\n        }\n      ]\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MessageAttachment\"\n      },\n      \"description\": \"Array of message attachments\",\n      \"example\": [\n        {\n          \"\
  filename\": \"Example Name\",\n          \"content\": \"example_value\",\n          \"content_type\": \"example_value\",\n          \"content_id\": \"500123\"\n        }\n      ]\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Email headers as key-value pairs (values are arrays to handle multiple headers with same name)\",\n      \"example\": {\n        \"Content-Type\": [\n          \"text/html; charset=utf-8\"\n        ],\n        \"X-Custom-Header\": [\n          \"value1\",\n          \"value2\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"parts\",\n    \"attachments\",\n    \"headers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-content-parsed-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: MessageContentParsed
---
