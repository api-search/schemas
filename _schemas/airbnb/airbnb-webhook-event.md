---
description: The envelope schema for all webhook event notifications sent by the Airbnb platform to partner endpoints, including event metadata and typed payloads.
layout: schema
name: Airbnb Webhook Event
properties_list:
- description: A unique identifier for this webhook event, used for idempotency and deduplication.
  name: event_id
  type: string
- description: The type of event that triggered the webhook notification.
  name: event_type
  type: string
- description: The ISO 8601 timestamp when the event occurred.
  name: timestamp
  type: string
- description: The API version used for the webhook payload format.
  name: api_version
  type: string
- description: The event-specific payload data. Structure varies by event_type.
  name: data
  type: object
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-webhook-event-schema.json
slug: airbnb-webhook-event
source_filename: airbnb-webhook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.airbnb.com/schemas/airbnb/webhook-event.json\",\n  \"title\": \"Airbnb Webhook Event\",\n  \"description\": \"The envelope schema for all webhook event notifications sent by the Airbnb platform to partner endpoints, including event metadata and typed payloads.\",\n  \"type\": \"object\",\n  \"required\": [\"event_id\", \"event_type\", \"timestamp\", \"data\"],\n  \"properties\": {\n    \"event_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this webhook event, used for idempotency and deduplication.\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that triggered the webhook notification.\",\n      \"enum\": [\n        \"reservation.created\",\n        \"reservation.confirmed\",\n        \"reservation.cancelled\",\n        \"reservation.updated\",\n        \"reservation.checked_in\",\n  \
  \      \"reservation.checked_out\",\n        \"message.created\",\n        \"review.submitted\",\n        \"calendar.updated\",\n        \"listing.updated\",\n        \"pricing.updated\",\n        \"booking.created\",\n        \"booking.confirmed\",\n        \"booking.cancelled\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the event occurred.\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"The API version used for the webhook payload format.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The event-specific payload data. Structure varies by event_type.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-webhook-event-schema.json
tags: []
title: Airbnb Webhook Event
---
