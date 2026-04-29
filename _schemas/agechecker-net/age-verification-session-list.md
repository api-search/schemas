---
description: SessionList schema from AgeChecker.Net API
layout: schema
name: SessionList
properties_list:
- description: ''
  name: sessions
  type: array
- description: Total number of matching sessions.
  name: total
  type: integer
- description: Page size.
  name: limit
  type: integer
- description: Page offset.
  name: offset
  type: integer
provider_name: AgeChecker.Net
provider_slug: agechecker-net
schema_file: json-schema/age-verification-session-list-schema.json
slug: age-verification-session-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-session-list-schema.json\",\n  \"title\": \"SessionList\",\n  \"description\": \"SessionList schema from AgeChecker.Net API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Session\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching sessions.\",\n      \"example\": 1\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Page size.\",\n      \"example\": 1\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Page offset.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-session-list-schema.json
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
title: SessionList
---
