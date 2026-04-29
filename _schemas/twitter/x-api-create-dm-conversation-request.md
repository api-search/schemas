---
description: CreateDmConversationRequest schema from X API v2
layout: schema
name: CreateDmConversationRequest
properties_list:
- description: The conversation type that is being created.
  name: conversation_type
  type: string
- description: ''
  name: message
  type: object
- description: Participants for the DM Conversation.
  name: participant_ids
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-create-dm-conversation-request-schema.json
slug: x-api-create-dm-conversation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-create-dm-conversation-request-schema.json\",\n  \"title\": \"CreateDmConversationRequest\",\n  \"description\": \"CreateDmConversationRequest schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conversation_type\": {\n      \"type\": \"string\",\n      \"description\": \"The conversation type that is being created.\",\n      \"enum\": [\n        \"Group\"\n      ]\n    },\n    \"message\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateTextMessageRequest\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CreateAttachmentsMessageRequest\"\n        }\n      ]\n    },\n    \"participant_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Participants for the DM Conversation.\",\n      \"minItems\": 2,\n      \"maxItems\"\
  : 49,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    }\n  },\n  \"required\": [\n    \"conversation_type\",\n    \"participant_ids\",\n    \"message\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-create-dm-conversation-request-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: CreateDmConversationRequest
---
