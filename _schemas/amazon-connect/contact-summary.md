---
description: Contains summary information about a contact.
layout: schema
name: ContactSummary
properties_list:
- description: The identifier of the contact.
  name: Id
  type: string
- description: The ARN of the contact.
  name: Arn
  type: string
- description: How the contact reached your contact center.
  name: Channel
  type: string
- description: Indicates how the contact was initiated.
  name: InitiationMethod
  type: string
- description: ''
  name: InitiationTimestamp
  type: string
- description: ''
  name: DisconnectTimestamp
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/contact-summary-schema.json
slug: contact-summary
source_filename: contact-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-summary-schema.json\",\n  \"title\": \"ContactSummary\",\n  \"description\": \"Contains summary information about a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-88888EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the contact.\"\n    },\n    \"Channel\": {\n      \"type\": \"string\",\n      \"description\": \"How the contact reached your contact center.\",\n      \"enum\": [\n        \"VOICE\",\n        \"CHAT\",\n        \"TASK\",\n        \"EMAIL\"\n      ],\n      \"example\": \"VOICE\"\n    },\n    \"InitiationMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates\
  \ how the contact was initiated.\",\n      \"example\": \"INBOUND\"\n    },\n    \"InitiationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DisconnectTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-summary-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ContactSummary
---
