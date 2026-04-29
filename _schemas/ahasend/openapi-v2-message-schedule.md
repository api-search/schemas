---
description: MessageSchedule schema from AhaSend API
layout: schema
name: MessageSchedule
properties_list:
- description: The time to make the first attempt for delivering the message (RFC3339 format)
  name: first_attempt
  type: string
- description: Expire and drop the message if not delivered by this time (RFC3339 format)
  name: expires
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-schedule-schema.json
slug: openapi-v2-message-schedule
source_filename: openapi-v2-message-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-schedule-schema.json\",\n  \"title\": \"MessageSchedule\",\n  \"description\": \"MessageSchedule schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_attempt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time to make the first attempt for delivering the message (RFC3339 format)\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"expires\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Expire and drop the message if not delivered by this time (RFC3339 format)\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"example\": {\n    \"first_attempt\": \"2023-12-25T10:30:00Z\",\n    \"expires\": \"2023-12-26T10:30:00Z\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-schedule-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: MessageSchedule
---
