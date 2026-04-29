---
description: Information about a configured webhook.
layout: schema
name: WebhookInfo
properties_list:
- description: The unique webhook identifier.
  name: id
  type: integer
- description: The webhook URL.
  name: url
  type: string
- description: A description of the webhook.
  name: description
  type: string
- description: The key used to generate webhook signatures for verifying webhook authenticity.
  name: auth_key
  type: string
- description: The events that trigger this webhook.
  name: events
  type: array
- description: When the webhook was created.
  name: created_at
  type: string
- description: When the webhook last fired.
  name: last_sent_at
  type: string
- description: Total number of event batches sent.
  name: batches_sent
  type: integer
- description: Total number of events sent.
  name: events_sent
  type: integer
- description: The last error received from the webhook URL.
  name: last_error
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-webhook-info-schema.json
slug: mailchimp-transactional-webhook-info
source_filename: mailchimp-transactional-webhook-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about a configured webhook.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique webhook identifier.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The webhook URL.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the webhook.\"\n    },\n    \"auth_key\": {\n      \"type\": \"string\",\n      \"description\": \"The key used to generate webhook signatures for verifying webhook authenticity.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"The events that trigger this webhook.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the webhook was created.\"\n    },\n    \"last_sent_at\": {\n      \"type\": \"\
  string\",\n      \"description\": \"When the webhook last fired.\"\n    },\n    \"batches_sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of event batches sent.\"\n    },\n    \"events_sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of events sent.\"\n    },\n    \"last_error\": {\n      \"type\": \"string\",\n      \"description\": \"The last error received from the webhook URL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-webhook-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: WebhookInfo
---
