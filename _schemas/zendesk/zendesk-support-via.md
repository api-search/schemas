---
description: How the ticket or comment was created.
layout: schema
name: Via
properties_list:
- description: The channel the ticket or comment came through (e.g., web, email, api, chat, voice).
  name: channel
  type: string
- description: ''
  name: source
  type: object
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-via-schema.json
slug: zendesk-support-via
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Via\",\n  \"type\": \"object\",\n  \"description\": \"How the ticket or comment was created.\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The channel the ticket or comment came through (e.g., web, email, api, chat, voice).\"\n    },\n    \"source\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-via-schema.json
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
title: Via
---
