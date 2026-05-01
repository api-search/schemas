---
description: StartChatContactResponse schema from Amazon Connect Service API
layout: schema
name: StartChatContactResponse
properties_list:
- description: The identifier of the contact.
  name: ContactId
  type: string
- description: The identifier for a chat participant.
  name: ParticipantId
  type: string
- description: The token used by the chat participant to call CreateParticipantConnection.
  name: ParticipantToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/start-chat-contact-response-schema.json
slug: start-chat-contact-response
source_filename: start-chat-contact-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-chat-contact-response-schema.json\",\n  \"title\": \"StartChatContactResponse\",\n  \"description\": \"StartChatContactResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContactId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-88888EXAMPLE\"\n    },\n    \"ParticipantId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for a chat participant.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-99999EXAMPLE\"\n    },\n    \"ParticipantToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token used by the chat participant to call CreateParticipantConnection.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-chat-contact-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: StartChatContactResponse
---
