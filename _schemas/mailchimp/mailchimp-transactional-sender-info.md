---
description: Information and statistics for a sender address.
layout: schema
name: SenderInfo
properties_list:
- description: The sender email address.
  name: address
  type: string
- description: When the sender was first used.
  name: created_at
  type: string
- description: Total number of messages sent from this address.
  name: sent
  type: integer
- description: Total hard bounces.
  name: hard_bounces
  type: integer
- description: Total soft bounces.
  name: soft_bounces
  type: integer
- description: Total rejects.
  name: rejects
  type: integer
- description: Total spam complaints.
  name: complaints
  type: integer
- description: Total unsubscribes.
  name: unsubs
  type: integer
- description: Total opens.
  name: opens
  type: integer
- description: Total clicks.
  name: clicks
  type: integer
- description: Unique opens.
  name: unique_opens
  type: integer
- description: Unique clicks.
  name: unique_clicks
  type: integer
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-sender-info-schema.json
slug: mailchimp-transactional-sender-info
source_filename: mailchimp-transactional-sender-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SenderInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information and statistics for a sender address.\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"The sender email address.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the sender was first used.\"\n    },\n    \"sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of messages sent from this address.\"\n    },\n    \"hard_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total hard bounces.\"\n    },\n    \"soft_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total soft bounces.\"\n    },\n    \"rejects\": {\n      \"type\": \"integer\",\n      \"description\": \"Total rejects.\"\n    },\n    \"complaints\": {\n      \"type\": \"integer\",\n      \"description\": \"Total\
  \ spam complaints.\"\n    },\n    \"unsubs\": {\n      \"type\": \"integer\",\n      \"description\": \"Total unsubscribes.\"\n    },\n    \"opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total opens.\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total clicks.\"\n    },\n    \"unique_opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique opens.\"\n    },\n    \"unique_clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique clicks.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-sender-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: SenderInfo
---
