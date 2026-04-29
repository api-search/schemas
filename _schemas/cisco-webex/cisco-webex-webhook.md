---
description: Represents a webhook registration that receives real-time HTTP callbacks when specific events occur in Webex.
layout: schema
name: Cisco Webex Webhook
properties_list:
- description: Unique identifier for the webhook.
  name: id
  type: string
- description: A user-friendly name for the webhook.
  name: name
  type: string
- description: The URL that receives webhook POST requests.
  name: targetUrl
  type: string
- description: The resource type monitored by the webhook.
  name: resource
  type: string
- description: The event type monitored by the webhook.
  name: event
  type: string
- description: The filter expression for narrowing webhook scope.
  name: filter
  type: string
- description: Secret used for generating payload signatures for verification.
  name: secret
  type: string
- description: The current status of the webhook.
  name: status
  type: string
- description: Webhook ownership type.
  name: ownedBy
  type: string
- description: Organization ID of the webhook owner.
  name: orgId
  type: string
- description: Person ID of the webhook creator.
  name: createdBy
  type: string
- description: Application ID associated with the webhook.
  name: appId
  type: string
- description: Date and time the webhook was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-webhook-schema.json
slug: cisco-webex-webhook
source_filename: cisco-webex-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/webhook.json\",\n  \"title\": \"Cisco Webex Webhook\",\n  \"description\": \"Represents a webhook registration that receives real-time HTTP callbacks when specific events occur in Webex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the webhook.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the webhook.\"\n    },\n    \"targetUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that receives webhook POST requests.\"\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type monitored by the webhook.\",\n      \"enum\": [\"messages\", \"rooms\", \"memberships\", \"meetings\", \"recordings\", \"meetingParticipants\", \"\
  meetingTranscripts\", \"attachmentActions\", \"telephony_calls\"]\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The event type monitored by the webhook.\",\n      \"enum\": [\"created\", \"updated\", \"deleted\", \"started\", \"ended\", \"joined\", \"left\", \"migrated\", \"read\"]\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The filter expression for narrowing webhook scope.\"\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"Secret used for generating payload signatures for verification.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the webhook.\",\n      \"enum\": [\"active\", \"inactive\"]\n    },\n    \"ownedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook ownership type.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization ID of the webhook owner.\"\n   \
  \ },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Person ID of the webhook creator.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Application ID associated with the webhook.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the webhook was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"targetUrl\", \"resource\", \"event\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-webhook-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Webhook
---
