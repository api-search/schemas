---
description: The result of sending a message to a single recipient.
layout: schema
name: SendResult
properties_list:
- description: The recipient email address.
  name: email
  type: string
- description: The sending status for this recipient.
  name: status
  type: string
- description: The reason the message was rejected, if applicable.
  name: reject_reason
  type: string
- description: The reason the message was queued instead of sent immediately.
  name: queued_reason
  type: string
- description: The unique message ID for this recipient's message.
  name: _id
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-send-result-schema.json
slug: mailchimp-transactional-send-result
source_filename: mailchimp-transactional-send-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SendResult\",\n  \"type\": \"object\",\n  \"description\": \"The result of sending a message to a single recipient.\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient email address.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The sending status for this recipient.\"\n    },\n    \"reject_reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the message was rejected, if applicable.\"\n    },\n    \"queued_reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the message was queued instead of sent immediately.\"\n    },\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique message ID for this recipient's message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-send-result-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: SendResult
---
