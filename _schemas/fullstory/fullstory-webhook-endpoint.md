---
description: A configured webhook endpoint in FullStory that receives real-time event notifications. Endpoints define a destination URL, the event types to receive, and a signing secret for payload verification.
layout: schema
name: FullStory Webhook Endpoint
properties_list:
- description: Unique identifier for the webhook endpoint
  name: id
  type: string
- description: The destination URL that receives webhook event notifications
  name: url
  type: string
- description: The event types configured for this endpoint
  name: events
  type: array
- description: Secret used to sign webhook payloads for verification by the receiving application
  name: signingSecret
  type: string
- description: Whether the endpoint is actively receiving events
  name: enabled
  type: boolean
- description: Timestamp when the endpoint was created
  name: createdAt
  type: string
provider_name: FullStory
provider_slug: fullstory
schema_file: json-schema/fullstory-webhook-endpoint-schema.json
slug: fullstory-webhook-endpoint
source_filename: fullstory-webhook-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fullstory.com/schemas/fullstory/webhook-endpoint.json\",\n  \"title\": \"FullStory Webhook Endpoint\",\n  \"description\": \"A configured webhook endpoint in FullStory that receives real-time event notifications. Endpoints define a destination URL, the event types to receive, and a signing secret for payload verification.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"url\", \"events\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the webhook endpoint\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The destination URL that receives webhook event notifications\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"The event types configured for this endpoint\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EventTypeConfig\"\
  \n      }\n    },\n    \"signingSecret\": {\n      \"type\": \"string\",\n      \"description\": \"Secret used to sign webhook payloads for verification by the receiving application\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the endpoint is actively receiving events\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was created\"\n    }\n  },\n  \"$defs\": {\n    \"EventTypeConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a specific event type on a webhook endpoint\",\n      \"required\": [\"eventName\"],\n      \"properties\": {\n        \"eventName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the event type\",\n          \"enum\": [\n            \"segment.created\",\n            \"segment.trend.alert\",\n            \"recording.event.custom\",\n            \"note.created\"\
  \n          ]\n        },\n        \"subcategory\": {\n          \"type\": \"string\",\n          \"description\": \"Required subcategory for event types that support it, such as specifying which custom event to listen for\"\n        }\n      }\n    },\n    \"EventType\": {\n      \"type\": \"object\",\n      \"description\": \"A webhook event type available in FullStory\",\n      \"properties\": {\n        \"eventName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the event type\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the event type\"\n        },\n        \"hasSubcategories\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this event type requires a subcategory when configuring an endpoint\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/json-schema/fullstory-webhook-endpoint-schema.json
tags:
- Analytics
- Digital Experience
- Session Replay
- Webhooks
- Data Export
title: FullStory Webhook Endpoint
---
