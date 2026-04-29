---
description: Information about the bearer token used for authentication.
layout: schema
name: TokenIntrospection
properties_list:
- description: The unique identifier of the token.
  name: uuid
  type: string
- description: The features and permissions the token has access to.
  name: features
  type: array
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-token-introspection-schema.json
slug: 1password-events-token-introspection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-token-introspection-schema.json\",\n  \"title\": \"TokenIntrospection\",\n  \"description\": \"Information about the bearer token used for authentication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the token.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"The features and permissions the token has access to.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"signinattempts\",\n          \"itemusages\",\n          \"auditevents\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-token-introspection-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: TokenIntrospection
---
