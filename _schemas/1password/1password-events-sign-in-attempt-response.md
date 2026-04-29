---
description: The response containing sign-in attempt records and a cursor for pagination.
layout: schema
name: SignInAttemptResponse
properties_list:
- description: A cursor to use in the next request to continue fetching events.
  name: cursor
  type: string
- description: Whether there are more events available to fetch using the cursor.
  name: has_more
  type: boolean
- description: The list of sign-in attempt records.
  name: items
  type: array
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-sign-in-attempt-response-schema.json
slug: 1password-events-sign-in-attempt-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-sign-in-attempt-response-schema.json\",\n  \"title\": \"SignInAttemptResponse\",\n  \"description\": \"The response containing sign-in attempt records and a cursor for pagination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"A cursor to use in the next request to continue fetching events.\"\n    },\n    \"has_more\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are more events available to fetch using the cursor.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of sign-in attempt records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SignInAttempt\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-sign-in-attempt-response-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: SignInAttemptResponse
---
