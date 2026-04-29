---
description: ''
layout: schema
name: Message
properties_list:
- description: The unique identifier of the message.
  name: id
  type: string
- description: The identifier of the associated reservation.
  name: reservation_id
  type: string
- description: Whether the message was sent by the host or guest.
  name: sender_type
  type: string
- description: The text content of the message.
  name: message
  type: string
- description: The timestamp when the message was sent.
  name: created_at
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-message-schema.json
slug: airbnb-message
source_filename: airbnb-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-message-schema.json\",\n  \"title\": \"Message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the message.\"\n    },\n    \"reservation_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the associated reservation.\"\n    },\n    \"sender_type\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the message was sent by the host or guest.\",\n      \"enum\": [\n        \"host\",\n        \"guest\"\n      ]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the message.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the message\
  \ was sent.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-message-schema.json
tags: []
title: Message
---
