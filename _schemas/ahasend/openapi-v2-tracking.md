---
description: Tracking schema from AhaSend API
layout: schema
name: Tracking
properties_list:
- description: Whether to track opens
  name: open
  type: boolean
- description: Whether to track clicks
  name: click
  type: boolean
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-tracking-schema.json
slug: openapi-v2-tracking
source_filename: openapi-v2-tracking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-tracking-schema.json\",\n  \"title\": \"Tracking\",\n  \"description\": \"Tracking schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"open\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to track opens\",\n      \"example\": true\n    },\n    \"click\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to track clicks\",\n      \"example\": true\n    }\n  },\n  \"example\": {\n    \"open\": true,\n    \"click\": true\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-tracking-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Tracking
---
