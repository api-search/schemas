---
description: A message scheduled for future delivery.
layout: schema
name: ScheduledMessage
properties_list:
- description: The unique scheduled message ID.
  name: _id
  type: string
- description: When the scheduled message was created.
  name: created_at
  type: string
- description: When the message is scheduled to be sent.
  name: send_at
  type: string
- description: The sender email address.
  name: from_email
  type: string
- description: The recipient email address.
  name: to
  type: string
- description: The message subject line.
  name: subject
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-scheduled-message-schema.json
slug: mailchimp-transactional-scheduled-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduledMessage\",\n  \"type\": \"object\",\n  \"description\": \"A message scheduled for future delivery.\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique scheduled message ID.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the scheduled message was created.\"\n    },\n    \"send_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the message is scheduled to be sent.\"\n    },\n    \"from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The sender email address.\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient email address.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The message subject line.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-scheduled-message-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: ScheduledMessage
---
