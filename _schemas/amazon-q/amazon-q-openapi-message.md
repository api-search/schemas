---
description: Message schema from openapi
layout: schema
name: Message
properties_list:
- description: The unique identifier of the message.
  name: messageId
  type: string
- description: The content of the message.
  name: body
  type: string
- description: The type of message.
  name: type
  type: string
- description: The time the message was sent.
  name: time
  type: string
provider_name: Amazon Q
provider_slug: amazon-q
schema_file: json-schema/amazon-q-openapi-message-schema.json
slug: amazon-q-openapi-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Message schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the message.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the message.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"USER\",\n        \"SYSTEM\"\n      ],\n      \"description\": \"The type of message.\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the message was sent.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-message-schema.json
tags:
- Artificial Intelligence
- Assistant
- AWS
- Enterprise
- Generative AI
title: Message
---
