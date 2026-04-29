---
description: Session schema from AgeChecker.Net API
layout: schema
name: Session
properties_list:
- description: Unique session identifier.
  name: session_id
  type: string
- description: Current session status.
  name: status
  type: string
- description: Verification result.
  name: result
  type: string
- description: Whether age was verified.
  name: age_verified
  type: boolean
- description: Whether photo ID was required.
  name: requires_photo_id
  type: boolean
- description: When the session was created.
  name: created_at
  type: string
- description: When the session was completed.
  name: completed_at
  type: string
provider_name: AgeChecker.Net
provider_slug: agechecker-net
schema_file: json-schema/age-verification-session-schema.json
slug: age-verification-session
source_filename: age-verification-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-session-schema.json\",\n  \"title\": \"Session\",\n  \"description\": \"Session schema from AgeChecker.Net API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique session identifier.\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"completed\",\n        \"expired\"\n      ],\n      \"description\": \"Current session status.\",\n      \"example\": \"pending\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pass\",\n        \"fail\"\n      ],\n      \"description\": \"Verification result.\",\n      \"example\": \"pass\"\n    },\n    \"age_verified\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether age was verified.\",\n      \"example\": true\n    },\n    \"requires_photo_id\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether photo ID was required.\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the session was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the session was completed.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-session-schema.json
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
title: Session
---
