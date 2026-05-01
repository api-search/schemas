---
description: Contains information about a contact.
layout: schema
name: Contact
properties_list:
- description: The Amazon Resource Name (ARN) for the contact.
  name: Arn
  type: string
- description: The identifier for the contact.
  name: Id
  type: string
- description: If this contact is related to other contacts, this is the ID of the initial contact.
  name: InitialContactId
  type: string
- description: If this contact is not the first contact, this is the ID of the previous contact.
  name: PreviousContactId
  type: string
- description: How the contact reached your contact center.
  name: Channel
  type: string
- description: ''
  name: QueueInfo
  type: object
- description: ''
  name: AgentInfo
  type: object
- description: Indicates how the contact was initiated.
  name: InitiationMethod
  type: string
- description: The date and time this contact was initiated.
  name: InitiationTimestamp
  type: string
- description: The timestamp when the customer endpoint disconnected from Amazon Connect.
  name: DisconnectTimestamp
  type: string
- description: The timestamp when contact was last updated.
  name: LastUpdateTimestamp
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/contact-schema.json
slug: contact
source_filename: contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contains information about a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the contact.\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the contact.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-88888EXAMPLE\"\n    },\n    \"InitialContactId\": {\n      \"type\": \"string\",\n      \"description\": \"If this contact is related to other contacts, this is the ID of the initial contact.\"\n    },\n    \"PreviousContactId\": {\n      \"type\": \"string\",\n      \"description\": \"If this contact is not the first contact, this is the ID of the previous contact.\"\n  \
  \  },\n    \"Channel\": {\n      \"type\": \"string\",\n      \"description\": \"How the contact reached your contact center.\",\n      \"enum\": [\n        \"VOICE\",\n        \"CHAT\",\n        \"TASK\",\n        \"EMAIL\"\n      ],\n      \"example\": \"VOICE\"\n    },\n    \"QueueInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\"\n        },\n        \"EnqueueTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"AgentInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\"\n        },\n        \"ConnectedToAgentTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"InitiationMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates how the contact was initiated.\",\n      \"enum\": [\n        \"INBOUND\",\n       \
  \ \"OUTBOUND\",\n        \"TRANSFER\",\n        \"QUEUE_TRANSFER\",\n        \"CALLBACK\",\n        \"API\"\n      ],\n      \"example\": \"INBOUND\"\n    },\n    \"InitiationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time this contact was initiated.\"\n    },\n    \"DisconnectTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the customer endpoint disconnected from Amazon Connect.\"\n    },\n    \"LastUpdateTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when contact was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: Contact
---
