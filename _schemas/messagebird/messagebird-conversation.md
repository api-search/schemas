---
description: Represents an omnichannel conversation thread in the MessageBird Conversations API, consolidating messages from multiple channels into a single contact interaction.
layout: schema
name: MessageBird Conversation
properties_list:
- description: The unique identifier of the conversation.
  name: id
  type: string
- description: The unique identifier of the contact associated with this conversation.
  name: contactId
  type: string
- description: ''
  name: contact
  type: object
- description: The messaging channels used in this conversation.
  name: channels
  type: array
- description: The status of the conversation.
  name: status
  type: string
- description: The date and time when the conversation was created.
  name: createdDatetime
  type: string
- description: The date and time when the conversation was last updated.
  name: updatedDatetime
  type: string
- description: The date and time of the last received message.
  name: lastReceivedDatetime
  type: string
- description: The identifier of the last channel used in the conversation.
  name: lastUsedChannelId
  type: string
provider_name: messagebird
provider_slug: messagebird
schema_file: json-schema/messagebird-conversation-schema.json
slug: messagebird-conversation
source_filename: messagebird-conversation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/messagebird/conversation.json\",\n  \"title\": \"MessageBird Conversation\",\n  \"description\": \"Represents an omnichannel conversation thread in the MessageBird Conversations API, consolidating messages from multiple channels into a single contact interaction.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the conversation.\"\n    },\n    \"contactId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the contact associated with this conversation.\"\n    },\n    \"contact\": {\n      \"$ref\": \"#/$defs/Contact\"\n    },\n    \"channels\": {\n      \"type\": \"array\",\n      \"description\": \"The messaging channels used in this conversation.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Channel\"\
  \n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the conversation.\",\n      \"enum\": [\"active\", \"archived\"]\n    },\n    \"createdDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the conversation was created.\"\n    },\n    \"updatedDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the conversation was last updated.\"\n    },\n    \"lastReceivedDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last received message.\"\n    },\n    \"lastUsedChannelId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the last channel used in the conversation.\"\n    }\n  },\n  \"$defs\": {\n    \"Contact\": {\n      \"type\": \"object\",\n      \"description\": \"A contact associated with\
  \ one or more conversations.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the contact.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the contact resource.\"\n        },\n        \"msisdn\": {\n          \"type\": \"string\",\n          \"description\": \"The phone number of the contact in international format.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the contact.\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"The first name of the contact.\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"The last name of the contact.\"\n        },\n        \"customDetails\": {\n          \"type\": \"object\",\n          \"description\"\
  : \"Custom details associated with the contact.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createdDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the contact was created.\"\n        },\n        \"updatedDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the contact was last updated.\"\n        }\n      }\n    },\n    \"Channel\": {\n      \"type\": \"object\",\n      \"description\": \"A messaging channel through which conversations take place.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the channel.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the channel.\"\n        },\n        \"platformId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The messaging platform.\",\n          \"enum\": [\"sms\", \"whatsapp\", \"facebook\", \"telegram\", \"line\", \"wechat\", \"email\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the channel.\",\n          \"enum\": [\"active\", \"inactive\", \"pending\"]\n        },\n        \"createdDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the channel was created.\"\n        },\n        \"updatedDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the channel was last updated.\"\n        }\n      }\n    },\n    \"ConversationMessage\": {\n      \"type\": \"object\",\n      \"description\": \"A message within a conversation.\",\n      \"properties\": {\n        \"id\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"The unique identifier of the message.\"\n        },\n        \"conversationId\": {\n          \"type\": \"string\",\n          \"description\": \"The conversation this message belongs to.\"\n        },\n        \"channelId\": {\n          \"type\": \"string\",\n          \"description\": \"The channel through which the message was sent.\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"The messaging platform.\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient identifier.\"\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"The sender identifier.\"\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"description\": \"The direction of the message.\",\n          \"enum\": [\"sent\", \"received\"]\n        },\n        \"status\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The delivery status.\",\n          \"enum\": [\"accepted\", \"pending\", \"sent\", \"delivered\", \"read\", \"failed\", \"deleted\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of content.\",\n          \"enum\": [\"text\", \"image\", \"video\", \"audio\", \"file\", \"location\", \"hsm\"]\n        },\n        \"content\": {\n          \"type\": \"object\",\n          \"description\": \"The message content, structure depends on type.\"\n        },\n        \"createdDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the message was created.\"\n        },\n        \"updatedDatetime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the message was last updated.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/json-schema/messagebird-conversation-schema.json
tags: []
title: MessageBird Conversation
---
