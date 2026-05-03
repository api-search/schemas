---
description: Represents a conversational session with an Einstein Bot, including messages, status, and session metadata.
layout: schema
name: Einstein Bot Session
properties_list:
- description: Unique session identifier.
  name: sessionId
  type: string
- description: ID of the Einstein Bot handling the session.
  name: botId
  type: string
- description: Current status of the session.
  name: status
  type: string
- description: Timestamp when the session was created.
  name: createdDate
  type: string
- description: Timestamp of the last activity in the session.
  name: lastActiveDate
  type: string
- description: External key associated with the session.
  name: externalSessionKey
  type: string
- description: Messages exchanged during the session.
  name: messages
  type: array
- description: Whether the session has ended.
  name: sessionEnded
  type: boolean
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schema_file: json-schema/salesforce-einstein-bot-session-schema.json
slug: salesforce-einstein-bot-session
source_filename: salesforce-einstein-bot-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/salesforce-einstein/json-schema/salesforce-einstein-bot-session-schema.json\",\n  \"title\": \"Einstein Bot Session\",\n  \"description\": \"Represents a conversational session with an Einstein Bot, including messages, status, and session metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique session identifier.\"\n    },\n    \"botId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the Einstein Bot handling the session.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the session.\",\n      \"enum\": [\"Active\", \"Ended\", \"Transferred\"]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the session was created.\"\n    },\n\
  \    \"lastActiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last activity in the session.\"\n    },\n    \"externalSessionKey\": {\n      \"type\": \"string\",\n      \"description\": \"External key associated with the session.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Messages exchanged during the session.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BotMessage\"\n      }\n    },\n    \"sessionEnded\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the session has ended.\"\n    }\n  },\n  \"required\": [\"sessionId\", \"botId\", \"status\"],\n  \"$defs\": {\n    \"BotMessage\": {\n      \"type\": \"object\",\n      \"description\": \"A message in an Einstein Bot conversation.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of bot message.\",\n          \"enum\": [\n           \
  \ \"Text\",\n            \"Choices\",\n            \"Transfer\",\n            \"EscalateToAgent\",\n            \"SessionEnded\"\n          ]\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Text content of the message.\"\n        },\n        \"sender\": {\n          \"type\": \"string\",\n          \"description\": \"Who sent the message.\",\n          \"enum\": [\"User\", \"Bot\"]\n        },\n        \"choices\": {\n          \"type\": \"array\",\n          \"description\": \"Available choices for choice-type messages.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"index\": {\n                \"type\": \"integer\"\n              }\n            },\n            \"required\": [\"label\"]\n          }\n        },\n\
  \        \"sequenceId\": {\n          \"type\": \"integer\",\n          \"description\": \"Message sequence number.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the message was sent.\"\n        }\n      },\n      \"required\": [\"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/json-schema/salesforce-einstein-bot-session-schema.json
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
title: Einstein Bot Session
---
