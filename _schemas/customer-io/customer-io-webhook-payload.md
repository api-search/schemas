---
description: The payload format for Customer.io reporting webhook events. These events are sent via HTTP POST to your configured webhook endpoint when message activity occurs, such as sends, deliveries, opens, clicks, and bounces.
layout: schema
name: Customer.io Reporting Webhook Payload
properties_list:
- description: A unique identifier for this webhook event, used for deduplication.
  name: event_id
  type: string
- description: The type of message activity that triggered this webhook event.
  name: metric
  type: string
- description: A UNIX timestamp of when the event occurred.
  name: timestamp
  type: integer
- description: ''
  name: data
  type: object
provider_name: Customer.io
provider_slug: customer-io
schema_file: json-schema/customer-io-webhook-payload-schema.json
slug: customer-io-webhook-payload
source_filename: customer-io-webhook-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://customer.io/schemas/customer-io/webhook-payload.json\",\n  \"title\": \"Customer.io Reporting Webhook Payload\",\n  \"description\": \"The payload format for Customer.io reporting webhook events. These events are sent via HTTP POST to your configured webhook endpoint when message activity occurs, such as sends, deliveries, opens, clicks, and bounces.\",\n  \"type\": \"object\",\n  \"required\": [\"event_id\", \"metric\", \"timestamp\"],\n  \"properties\": {\n    \"event_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this webhook event, used for deduplication.\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"The type of message activity that triggered this webhook event.\",\n      \"enum\": [\n        \"sent\",\n        \"delivered\",\n        \"opened\",\n        \"clicked\",\n        \"bounced\",\n        \"spammed\"\
  ,\n        \"dropped\",\n        \"unsubscribed\",\n        \"converted\",\n        \"failed\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"A UNIX timestamp of when the event occurred.\"\n    },\n    \"data\": {\n      \"$ref\": \"#/$defs/WebhookEventData\"\n    }\n  },\n  \"$defs\": {\n    \"WebhookEventData\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed data about the message activity event.\",\n      \"properties\": {\n        \"customer_id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the customer who received the message.\"\n        },\n        \"email_address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address the message was sent to.\"\n        },\n        \"delivery_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique delivery identifier for the message. Referenced in the\
  \ X-CIO-Delivery-ID header.\"\n        },\n        \"action_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The campaign action identifier that generated the message.\"\n        },\n        \"campaign_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The campaign identifier that the message belongs to.\"\n        },\n        \"newsletter_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The newsletter identifier, if the message was part of a newsletter.\"\n        },\n        \"broadcast_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The broadcast identifier, if the message was triggered by a broadcast.\"\n        },\n        \"subject\": {\n          \"type\": \"string\",\n          \"description\": \"The email subject line.\"\n        },\n        \"template_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The template identifier used for the message.\"\n        },\n   \
  \     \"content_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The content variant identifier for A/B test variants.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL that was clicked. Only present for click events.\"\n        },\n        \"link_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The link identifier within the message. Only present for click events.\"\n        },\n        \"device_id\": {\n          \"type\": \"string\",\n          \"description\": \"The device identifier for push notification events.\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"The device platform for push notification events.\",\n          \"enum\": [\"ios\", \"android\"]\n        },\n        \"from_phone\": {\n          \"type\": \"string\",\n          \"description\": \"The sender phone number for SMS events.\"\n\
  \        },\n        \"to_phone\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient phone number for SMS events.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/json-schema/customer-io-webhook-payload-schema.json
tags:
- Behavioral Data
- Broadcasts
- Campaigns
- CDP
- Customer Data
- Customer Data Platform
- Data Ingestion
- Email
- Event Tracking
- Marketing Automation
- Messaging
- Push Notifications
- Segments
- SMS
- Transactional Email
title: Customer.io Reporting Webhook Payload
---
