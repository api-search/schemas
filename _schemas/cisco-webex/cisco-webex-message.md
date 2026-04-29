---
description: Represents a message posted in a Webex room, including text, markdown, files, and adaptive card attachments.
layout: schema
name: Cisco Webex Message
properties_list:
- description: Unique identifier for the message.
  name: id
  type: string
- description: The parent message ID if this is a threaded reply.
  name: parentId
  type: string
- description: The room ID where the message was posted.
  name: roomId
  type: string
- description: The type of room.
  name: roomType
  type: string
- description: The plain text content of the message.
  name: text
  type: string
- description: The message content in markdown format.
  name: markdown
  type: string
- description: The rendered HTML content of the message.
  name: html
  type: string
- description: Public URLs for files attached to the message.
  name: files
  type: array
- description: The person ID of the message author.
  name: personId
  type: string
- description: The email address of the message author.
  name: personEmail
  type: string
- description: Person IDs of those mentioned in the message.
  name: mentionedPeople
  type: array
- description: Group names mentioned in the message.
  name: mentionedGroups
  type: array
- description: Adaptive card attachments on the message.
  name: attachments
  type: array
- description: Whether the message is a voice clip.
  name: isVoiceClip
  type: boolean
- description: The date and time the message was created.
  name: created
  type: string
- description: The date and time the message was last updated.
  name: updated
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-message-schema.json
slug: cisco-webex-message
source_filename: cisco-webex-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/message.json\",\n  \"title\": \"Cisco Webex Message\",\n  \"description\": \"Represents a message posted in a Webex room, including text, markdown, files, and adaptive card attachments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the message.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The parent message ID if this is a threaded reply.\"\n    },\n    \"roomId\": {\n      \"type\": \"string\",\n      \"description\": \"The room ID where the message was posted.\"\n    },\n    \"roomType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of room.\",\n      \"enum\": [\"direct\", \"group\"]\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text content of the message.\"\
  ,\n      \"maxLength\": 7439\n    },\n    \"markdown\": {\n      \"type\": \"string\",\n      \"description\": \"The message content in markdown format.\",\n      \"maxLength\": 7439\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"The rendered HTML content of the message.\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"Public URLs for files attached to the message.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID of the message author.\"\n    },\n    \"personEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the message author.\"\n    },\n    \"mentionedPeople\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs of those mentioned in the message.\",\n      \"items\": {\n        \"type\": \"string\"\n\
  \      }\n    },\n    \"mentionedGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Group names mentioned in the message.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"Adaptive card attachments on the message.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"contentType\": {\n            \"type\": \"string\",\n            \"description\": \"The content type of the attachment.\"\n          },\n          \"content\": {\n            \"type\": \"object\",\n            \"description\": \"Adaptive card content object.\"\n          }\n        }\n      }\n    },\n    \"isVoiceClip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the message is a voice clip.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was created.\"\
  \n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"roomId\", \"personId\", \"created\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-message-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Message
---
