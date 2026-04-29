---
description: Message schema from Bandwidth messaging API
layout: schema
name: Message
properties_list:
- description: The unique identifier for the message
  name: id
  type: string
- description: The Bandwidth phone number that owns the message
  name: owner
  type: string
- description: The application ID associated with this message
  name: applicationId
  type: string
- description: The time the message was created
  name: time
  type: string
- description: The number of segments the message was split into
  name: segmentCount
  type: integer
- description: The direction of the message
  name: direction
  type: string
- description: The destination phone numbers
  name: to
  type: array
- description: The source phone number
  name: from
  type: string
- description: Media URLs attached to the message
  name: media
  type: array
- description: The text content of the message
  name: text
  type: string
- description: Custom tag attached to the message
  name: tag
  type: string
- description: The priority of the message
  name: priority
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-message-schema.json
slug: messaging-message
source_filename: messaging-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Message schema from Bandwidth messaging API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth phone number that owns the message\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID associated with this message\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the message was created\"\n    },\n    \"segmentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of segments the\
  \ message was split into\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"in\",\n        \"out\"\n      ],\n      \"description\": \"The direction of the message\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The destination phone numbers\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The source phone number\"\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"Media URLs attached to the message\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the message\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Custom tag attached to the message\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\n   \
  \     \"default\",\n        \"high\"\n      ],\n      \"description\": \"The priority of the message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-message-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Message
---
