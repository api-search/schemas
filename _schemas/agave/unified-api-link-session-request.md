---
description: Request payload for creating an Agave Link session.
layout: schema
name: LinkSessionRequest
properties_list:
- description: Unique identifier for the user or entity linking their account.
  name: reference_id
  type: string
- description: URL to redirect the user to after completing the link flow.
  name: redirect_url
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-link-session-request-schema.json
slug: unified-api-link-session-request
source_filename: unified-api-link-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-link-session-request-schema.json\",\n  \"title\": \"LinkSessionRequest\",\n  \"description\": \"Request payload for creating an Agave Link session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user or entity linking their account.\",\n      \"example\": \"user-789-procore\"\n    },\n    \"redirect_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to redirect the user to after completing the link flow.\",\n      \"example\": \"https://myapp.com/integration/callback\"\n    }\n  },\n  \"required\": [\n    \"reference_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-link-session-request-schema.json
tags:
- Accounting
- Construction
- Integration
title: LinkSessionRequest
---
