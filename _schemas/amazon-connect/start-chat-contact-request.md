---
description: StartChatContactRequest schema from Amazon Connect Service API
layout: schema
name: StartChatContactRequest
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: InstanceId
  type: string
- description: The identifier of the contact flow for initiating the chat.
  name: ContactFlowId
  type: string
- description: A custom key-value pair using an attribute map.
  name: Attributes
  type: object
- description: ''
  name: ParticipantDetails
  type: object
- description: ''
  name: InitialMessage
  type: object
- description: Idempotency token.
  name: ClientToken
  type: string
- description: The total duration of the newly started chat session.
  name: ChatDurationInMinutes
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/start-chat-contact-request-schema.json
slug: start-chat-contact-request
source_filename: start-chat-contact-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-chat-contact-request-schema.json\",\n  \"title\": \"StartChatContactRequest\",\n  \"description\": \"StartChatContactRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"ContactFlowId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow for initiating the chat.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"A custom key-value pair using an attribute map.\",\n      \"additionalProperties\": {\n        \"type\": \"\
  string\"\n      }\n    },\n    \"ParticipantDetails\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"DisplayName\"\n      ],\n      \"properties\": {\n        \"DisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the participant.\",\n          \"example\": \"Jane Smith\"\n        }\n      }\n    },\n    \"InitialMessage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ContentType\": {\n          \"type\": \"string\",\n          \"example\": \"text/plain\"\n        },\n        \"Content\": {\n          \"type\": \"string\",\n          \"example\": \"Hello, I need help with my order.\"\n        }\n      }\n    },\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"Idempotency token.\"\n    },\n    \"ChatDurationInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The total duration of the newly started chat session.\",\n      \"example\": 60\n    }\n  },\n  \"\
  required\": [\n    \"ContactFlowId\",\n    \"InstanceId\",\n    \"ParticipantDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-chat-contact-request-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: StartChatContactRequest
---
