---
description: A user registered in the Sendbird application.
layout: schema
name: Sendbird User
properties_list:
- description: Unique identifier of the user within the Sendbird application.
  name: user_id
  type: string
- description: Display nickname of the user shown in chat.
  name: nickname
  type: string
- description: URL of the user's profile image.
  name: profile_url
  type: string
- description: Whether the user is currently online.
  name: is_online
  type: boolean
- description: Whether the user account is active (not deactivated).
  name: is_active
  type: boolean
- description: Unix timestamp (milliseconds) of the user's last activity.
  name: last_seen_at
  type: integer
- description: Session token for the user. Returned when issue_access_token is true during creation.
  name: access_token
  type: string
- description: Custom metadata key-value pairs associated with the user.
  name: metadata
  type: object
- description: Unix timestamp (milliseconds) when the user was created.
  name: created_at
  type: integer
provider_name: Sendbird
provider_slug: sendbird
schema_file: json-schema/sendbird-user-schema.json
slug: sendbird-user
source_filename: sendbird-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sendbird/json-schema/sendbird-user-schema.json\",\n  \"title\": \"Sendbird User\",\n  \"description\": \"A user registered in the Sendbird application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user within the Sendbird application.\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Display nickname of the user shown in chat.\"\n    },\n    \"profile_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's profile image.\"\n    },\n    \"is_online\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is currently online.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active (not deactivated).\"\
  \n    },\n    \"last_seen_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (milliseconds) of the user's last activity.\"\n    },\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"Session token for the user. Returned when issue_access_token is true during creation.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata key-value pairs associated with the user.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (milliseconds) when the user was created.\"\n    }\n  },\n  \"required\": [\"user_id\", \"nickname\", \"profile_url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/json-schema/sendbird-user-schema.json
tags: []
title: Sendbird User
---
