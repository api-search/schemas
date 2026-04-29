---
description: Summary information about a sent message.
layout: schema
name: MessageInfo
properties_list:
- description: The Unix timestamp when the message was sent.
  name: ts
  type: integer
- description: The unique message ID.
  name: _id
  type: string
- description: The sender email address.
  name: sender
  type: string
- description: The template slug used, if any.
  name: template
  type: string
- description: The subject line of the message.
  name: subject
  type: string
- description: The recipient email address.
  name: email
  type: string
- description: Tags applied to the message.
  name: tags
  type: array
- description: The number of times the message was opened.
  name: opens
  type: integer
- description: Detailed open tracking events.
  name: opens_detail
  type: array
- description: The number of link clicks in the message.
  name: clicks
  type: integer
- description: Detailed click tracking events.
  name: clicks_detail
  type: array
- description: The current state of the message.
  name: state
  type: string
- description: Custom metadata attached to the message.
  name: metadata
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-message-info-schema.json
slug: mailchimp-transactional-message-info
source_filename: mailchimp-transactional-message-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageInfo\",\n  \"type\": \"object\",\n  \"description\": \"Summary information about a sent message.\",\n  \"properties\": {\n    \"ts\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp when the message was sent.\"\n    },\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique message ID.\"\n    },\n    \"sender\": {\n      \"type\": \"string\",\n      \"description\": \"The sender email address.\"\n    },\n    \"template\": {\n      \"type\": \"string\",\n      \"description\": \"The template slug used, if any.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject line of the message.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient email address.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to\
  \ the message.\"\n    },\n    \"opens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times the message was opened.\"\n    },\n    \"opens_detail\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed open tracking events.\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of link clicks in the message.\"\n    },\n    \"clicks_detail\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed click tracking events.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the message.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata attached to the message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-message-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: MessageInfo
---
