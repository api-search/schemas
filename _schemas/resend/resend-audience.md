---
description: JSON Schema for a Resend audience object used for managing contact lists.
layout: schema
name: Resend Audience
properties_list:
- description: The ID of the audience.
  name: id
  type: string
- description: The object type.
  name: object
  type: string
- description: The name of the audience.
  name: name
  type: string
- description: Date the audience was created.
  name: created_at
  type:
  - string
  - 'null'
provider_name: Resend
provider_slug: resend
schema_file: json-schema/resend-audience-schema.json
slug: resend-audience
source_filename: resend-audience-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resend/json-schema/resend-audience-schema.json\",\n  \"title\": \"Resend Audience\",\n  \"description\": \"JSON Schema for a Resend audience object used for managing contact lists.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the audience.\",\n      \"example\": \"78261eea-8f8b-4381-83c6-79fa7120f1cf\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"audience\",\n      \"description\": \"The object type.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the audience.\",\n      \"example\": \"Registered Users\"\n    },\n    \"created_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date the audience was created.\"\n    }\n  },\n  \"required\": [\"id\"\
  , \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/json-schema/resend-audience-schema.json
tags:
- Email
- Developer Tools
- Transactional Email
- Marketing Email
title: Resend Audience
---
