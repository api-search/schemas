---
description: Base schema for all webhook event payloads
layout: schema
name: WebhookEventBase
properties_list:
- description: The type of event that triggered this webhook
  name: eventType
  type: string
- description: Unique identifier for this event instance
  name: eventId
  type: string
- description: The Learning Manager account ID
  name: accountId
  type: string
- description: ISO 8601 timestamp when the event occurred
  name: timestamp
  type: string
- description: The system component that generated the event
  name: source
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-webhook-event-base-schema.json
slug: learning-manager-webhooks-webhook-event-base
source_filename: learning-manager-webhooks-webhook-event-base-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-webhook-event-base-schema.json\",\n  \"title\": \"WebhookEventBase\",\n  \"description\": \"Base schema for all webhook event payloads\",\n  \"type\": \"object\",\n  \"required\": [\n    \"eventType\",\n    \"eventId\",\n    \"accountId\",\n    \"timestamp\"\n  ],\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that triggered this webhook\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this event instance\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Learning Manager account ID\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"ISO 8601 timestamp when the event occurred\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The system component that generated the event\",\n      \"enum\": [\n        \"learner\",\n        \"admin\",\n        \"manager\",\n        \"system\",\n        \"api\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-webhook-event-base-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: WebhookEventBase
---
