---
description: Represents an activity event within a Webex organization, used for compliance and auditing purposes.
layout: schema
name: Cisco Webex Event
properties_list:
- description: Unique identifier for the event.
  name: id
  type: string
- description: The resource type affected by the event.
  name: resource
  type: string
- description: The type of event that occurred.
  name: type
  type: string
- description: The application ID that triggered the event.
  name: appId
  type: string
- description: The person ID who performed the action.
  name: actorId
  type: string
- description: The organization ID where the event occurred.
  name: orgId
  type: string
- description: Date and time the event occurred.
  name: created
  type: string
- description: The resource data at the time of the event.
  name: data
  type: object
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-event-schema.json
slug: cisco-webex-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/event.json\",\n  \"title\": \"Cisco Webex Event\",\n  \"description\": \"Represents an activity event within a Webex organization, used for compliance and auditing purposes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event.\"\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type affected by the event.\",\n      \"enum\": [\"attachmentActions\", \"files\", \"meetings\", \"meetingMessages\", \"meetingTranscripts\", \"memberships\", \"messages\", \"rooms\", \"tabs\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that occurred.\",\n      \"enum\": [\"created\", \"updated\", \"deleted\", \"ended\"]\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The application ID that triggered the event.\"\n    },\n    \"actorId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID who performed the action.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID where the event occurred.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the event occurred.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The resource data at the time of the event.\"\n    }\n  },\n  \"required\": [\"id\", \"resource\", \"type\", \"created\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-event-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Event
---
