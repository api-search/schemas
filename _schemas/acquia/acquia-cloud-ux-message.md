---
description: ux-message schema from Acquia Cloud API
layout: schema
name: Ux Message
properties_list:
- description: The message identifier.
  name: id
  type: integer
- description: The message unique identifier.
  name: uuid
  type: string
- description: The message title.
  name: title
  type: string
- description: The message body.
  name: body
  type: string
- description: The message url.
  name: url
  type: string
- description: ''
  name: filters
  type: object
- description: ''
  name: flags
  type: object
- description: The message priority weight.
  name: weight
  type: integer
- description: The UTC timestamp of when the message started.
  name: start_at
  type: string
- description: The UTC timestamp of when the message expires.
  name: expire_at
  type: string
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-ux-message-schema.json
slug: acquia-cloud-ux-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ux-message-schema.json\",\n  \"title\": \"Ux Message\",\n  \"description\": \"ux-message schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The message identifier.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The message unique identifier.\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The message title.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The message body.\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The message url.\",\n      \"nullable\": true\n    },\n    \"filters\"\
  : {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_ux-message-filters\"\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_ux-message-flags\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The message priority weight.\"\n    },\n    \"start_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC timestamp of when the message started.\"\n    },\n    \"expire_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC timestamp of when the message expires.\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"uuid\",\n    \"title\",\n    \"body\",\n    \"url\",\n    \"filters\",\n    \"flags\",\n    \"weight\",\n    \"start_at\",\n    \"expire_at\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ux-message-schema.json
tags:
- Content
- Experience
title: Ux Message
---
