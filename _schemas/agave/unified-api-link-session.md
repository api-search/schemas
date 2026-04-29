---
description: An Agave Link session token.
layout: schema
name: LinkSession
properties_list:
- description: Token to initialize the Agave Link component for the user.
  name: link_token
  type: string
- description: The reference ID associated with this session.
  name: reference_id
  type: string
- description: Timestamp when the link token expires.
  name: expires_at
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-link-session-schema.json
slug: unified-api-link-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-link-session-schema.json\",\n  \"title\": \"LinkSession\",\n  \"description\": \"An Agave Link session token.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"link_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token to initialize the Agave Link component for the user.\",\n      \"example\": \"link-token-abc123xyz456\"\n    },\n    \"reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"The reference ID associated with this session.\",\n      \"example\": \"user-789-procore\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the link token expires.\",\n      \"example\": \"2025-03-15T16:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-link-session-schema.json
tags:
- Accounting
- Construction
- Integration
title: LinkSession
---
