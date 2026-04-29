---
description: Represents a user involved in an event.
layout: schema
name: EventUser
properties_list:
- description: The unique identifier of the user.
  name: uuid
  type: string
- description: The name of the user.
  name: name
  type: string
- description: The email address of the user.
  name: email
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-event-user-schema.json
slug: 1password-events-event-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-user-schema.json\",\n  \"title\": \"EventUser\",\n  \"description\": \"Represents a user involved in an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-user-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: EventUser
---
