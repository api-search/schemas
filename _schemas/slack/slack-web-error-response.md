---
description: Standard error response from the Slack API.
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: ok
  type: boolean
- description: A short machine-readable error code such as "channel_not_found", "not_authed", "invalid_auth", "missing_scope", etc.
  name: error
  type: string
- description: ''
  name: response_metadata
  type: object
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-error-response-schema.json
slug: slack-web-error-response
source_filename: slack-web-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response from the Slack API.\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"boolean\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"A short machine-readable error code such as \\\"channel_not_found\\\", \\\"not_authed\\\", \\\"invalid_auth\\\", \\\"missing_scope\\\", etc.\"\n    },\n    \"response_metadata\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-error-response-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: ErrorResponse
---
