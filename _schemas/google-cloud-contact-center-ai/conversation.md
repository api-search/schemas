---
description: A conversation resource in Google Cloud Contact Center AI representing an interaction between a customer and an agent.
layout: schema
name: Conversation
properties_list:
- description: Resource name of the conversation.
  name: name
  type: string
- description: The source of the conversation data.
  name: dataSource
  type: object
- description: Timestamp when the conversation was created.
  name: createTime
  type: string
- description: Timestamp when the conversation was last updated.
  name: updateTime
  type: string
- description: Timestamp when the conversation started.
  name: startTime
  type: string
- description: Duration of the conversation in seconds format.
  name: duration
  type: string
- description: Number of turns in the conversation.
  name: turnCount
  type: integer
- description: Identifier of the agent in the conversation.
  name: agentId
  type: string
- description: Language code of the conversation.
  name: languageCode
  type: string
- description: User-defined labels for the conversation.
  name: labels
  type: object
- description: The conversation transcript.
  name: transcript
  type: object
provider_name: Google Cloud Contact Center AI
provider_slug: google-cloud-contact-center-ai
schema_file: json-schema/conversation.json
slug: conversation
source_filename: conversation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-contact-center-ai/refs/heads/main/json-schema/conversation.json\",\n  \"title\": \"Conversation\",\n  \"description\": \"A conversation resource in Google Cloud Contact Center AI representing an interaction between a customer and an agent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the conversation.\"\n    },\n    \"dataSource\": {\n      \"type\": \"object\",\n      \"description\": \"The source of the conversation data.\",\n      \"properties\": {\n        \"gcsSource\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"audioUri\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Storage URI for the audio file.\"\n            },\n            \"transcriptUri\": {\n              \"\
  type\": \"string\",\n              \"description\": \"Cloud Storage URI for the transcript.\"\n            }\n          }\n        },\n        \"dialogflowSource\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"dialogflowConversation\": {\n              \"type\": \"string\",\n              \"description\": \"Dialogflow conversation resource name.\"\n            }\n          }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the conversation was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the conversation was last updated.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the conversation started.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Duration of the conversation in seconds format.\"\n    },\n    \"turnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of turns in the conversation.\"\n    },\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the agent in the conversation.\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"Language code of the conversation.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined labels for the conversation.\"\n    },\n    \"transcript\": {\n      \"type\": \"object\",\n      \"description\": \"The conversation transcript.\",\n      \"properties\": {\n        \"transcriptSegments\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"text\": {\n                \"type\"\
  : \"string\"\n              },\n              \"confidence\": {\n                \"type\": \"number\"\n              },\n              \"segmentParticipant\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"role\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"ROLE_UNSPECIFIED\", \"HUMAN_AGENT\", \"AUTOMATED_AGENT\", \"END_USER\"]\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-contact-center-ai/refs/heads/main/json-schema/conversation.json
tags:
- AI
- Contact Center
- Conversations
- Customer Service
- Google Cloud
- Virtual Agents
title: Conversation
---
