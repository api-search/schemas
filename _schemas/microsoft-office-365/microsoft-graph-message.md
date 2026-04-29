---
description: A message in a mailFolder. Contains the message subject, body, sender, recipients, and other metadata.
layout: schema
name: Message
properties_list:
- description: Unique identifier for the message.
  name: id
  type: string
- description: The subject of the message.
  name: subject
  type: string
- description: The first 255 characters of the message body in text format.
  name: bodyPreview
  type: string
- description: The To recipients for the message.
  name: toRecipients
  type: array
- description: The Cc recipients for the message.
  name: ccRecipients
  type: array
- description: The Bcc recipients for the message.
  name: bccRecipients
  type: array
- description: The email addresses to use when replying.
  name: replyTo
  type: array
- description: The ID of the conversation the email belongs to.
  name: conversationId
  type: string
- description: The index of the message in the conversation.
  name: conversationIndex
  type: string
- description: The date and time the message was received.
  name: receivedDateTime
  type: string
- description: The date and time the message was sent.
  name: sentDateTime
  type: string
- description: The date and time the message was created.
  name: createdDateTime
  type: string
- description: The date and time the message was last changed.
  name: lastModifiedDateTime
  type: string
- description: Indicates whether the message has attachments.
  name: hasAttachments
  type: boolean
- description: The message ID in RFC2822 format.
  name: internetMessageId
  type: string
- description: The importance of the message.
  name: importance
  type: string
- description: Indicates whether the message has been read.
  name: isRead
  type: boolean
- description: Indicates whether the message is a draft.
  name: isDraft
  type: boolean
- description: Indicates whether a delivery receipt is requested.
  name: isDeliveryReceiptRequested
  type: boolean
- description: Indicates whether a read receipt is requested.
  name: isReadReceiptRequested
  type: boolean
- description: The categories associated with the message.
  name: categories
  type: array
- description: The unique identifier for the message's parent mailFolder.
  name: parentFolderId
  type: string
- description: The URL to open the message in Outlook on the web.
  name: webLink
  type: string
- description: The classification of the message based on inferred relevance.
  name: inferenceClassification
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-message-schema.json
slug: microsoft-graph-message
source_filename: microsoft-graph-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Message\",\n  \"type\": \"object\",\n  \"description\": \"A message in a mailFolder. Contains the message subject, body, sender, recipients, and other metadata.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the message.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the message.\"\n    },\n    \"bodyPreview\": {\n      \"type\": \"string\",\n      \"description\": \"The first 255 characters of the message body in text format.\"\n    },\n    \"toRecipients\": {\n      \"type\": \"array\",\n      \"description\": \"The To recipients for the message.\"\n    },\n    \"ccRecipients\": {\n      \"type\": \"array\",\n      \"description\": \"The Cc recipients for the message.\"\n    },\n    \"bccRecipients\": {\n      \"type\": \"array\",\n      \"description\": \"The Bcc recipients\
  \ for the message.\"\n    },\n    \"replyTo\": {\n      \"type\": \"array\",\n      \"description\": \"The email addresses to use when replying.\"\n    },\n    \"conversationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the conversation the email belongs to.\"\n    },\n    \"conversationIndex\": {\n      \"type\": \"string\",\n      \"description\": \"The index of the message in the conversation.\"\n    },\n    \"receivedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the message was received.\"\n    },\n    \"sentDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the message was sent.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the message was created.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the message was last changed.\"\n    },\n    \"hasAttachments\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has attachments.\"\n    },\n    \"internetMessageId\": {\n      \"type\": \"string\",\n      \"description\": \"The message ID in RFC2822 format.\"\n    },\n    \"importance\": {\n      \"type\": \"string\",\n      \"description\": \"The importance of the message.\"\n    },\n    \"isRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has been read.\"\n    },\n    \"isDraft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message is a draft.\"\n    },\n    \"isDeliveryReceiptRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a delivery receipt is requested.\"\n    },\n    \"isReadReceiptRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a read receipt is requested.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"The categories associated with the message.\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message's parent mailFolder.\"\n    },\n    \"webLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to open the message in Outlook on the web.\"\n    },\n    \"inferenceClassification\": {\n      \"type\": \"string\",\n      \"description\": \"The classification of the message based on inferred relevance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-message-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: Message
---
