---
description: The full content of a sent message.
layout: schema
name: MessageContent
properties_list:
- description: Unix timestamp of when the message was sent.
  name: ts
  type: integer
- description: The unique message ID.
  name: _id
  type: string
- description: The sender email address.
  name: from_email
  type: string
- description: The sender display name.
  name: from_name
  type: string
- description: The message subject line.
  name: subject
  type: string
- description: The primary recipient.
  name: to
  type: object
- description: Tags applied to the message.
  name: tags
  type: array
- description: The full message headers.
  name: headers
  type: object
- description: The plain-text body of the message.
  name: text
  type: string
- description: The HTML body of the message.
  name: html
  type: string
- description: File attachments included in the message.
  name: attachments
  type: array
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-message-content-schema.json
slug: mailchimp-transactional-message-content
source_filename: mailchimp-transactional-message-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageContent\",\n  \"type\": \"object\",\n  \"description\": \"The full content of a sent message.\",\n  \"properties\": {\n    \"ts\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the message was sent.\"\n    },\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique message ID.\"\n    },\n    \"from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The sender email address.\"\n    },\n    \"from_name\": {\n      \"type\": \"string\",\n      \"description\": \"The sender display name.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The message subject line.\"\n    },\n    \"to\": {\n      \"type\": \"object\",\n      \"description\": \"The primary recipient.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the message.\"\n    },\n\
  \    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"The full message headers.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The plain-text body of the message.\"\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML body of the message.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"File attachments included in the message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-message-content-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: MessageContent
---
