---
description: Message schema from AhaSend API
layout: schema
name: Message
properties_list: []
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-schema.json
slug: openapi-v2-message
source_filename: openapi-v2-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Message schema from AhaSend API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/MessageSummary\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"Original, raw email content (RFC822 format) - may be null if the message content is not available.\"\n        },\n        \"content_parsed\": {\n          \"$ref\": \"#/components/schemas/MessageContentParsed\",\n          \"description\": \"Parsed and structured message content including parts, attachments, and headers - may be null if the message content is not available.\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Message
---
