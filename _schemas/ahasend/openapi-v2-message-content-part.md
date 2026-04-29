---
description: MessageContentPart schema from AhaSend API
layout: schema
name: MessageContentPart
properties_list:
- description: MIME content type (e.g., "text/plain", "text/html")
  name: content_type
  type: string
- description: The actual content for this part
  name: content
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-content-part-schema.json
slug: openapi-v2-message-content-part
source_filename: openapi-v2-message-content-part-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-content-part-schema.json\",\n  \"title\": \"MessageContentPart\",\n  \"description\": \"MessageContentPart schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME content type (e.g., \\\"text/plain\\\", \\\"text/html\\\")\",\n      \"example\": \"text/html\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The actual content for this part\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"content_type\",\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-content-part-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: MessageContentPart
---
