---
description: A Zesty.io user account with profile information, authentication credentials, and role assignments across instances.
layout: schema
name: Zesty User
properties_list:
- description: The Zesty Universal Identifier for the user.
  name: ZUID
  type: string
- description: The user's first name.
  name: firstName
  type: string
- description: The user's last name.
  name: lastName
  type: string
- description: The user's email address.
  name: email
  type: string
- description: Timestamp when the user was created.
  name: createdAt
  type: string
- description: Timestamp when the user was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/user.json\",\n  \"title\": \"Zesty User\",\n  \"description\": \"A Zesty.io user account with profile information, authentication credentials, and role assignments across instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's first name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's last name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the\
  \ user was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"email\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/user.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty User
---
