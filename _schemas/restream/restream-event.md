---
description: A Restream live streaming event, which can be scheduled, in-progress, or historical.
layout: schema
name: Event
properties_list:
- description: Unique event identifier
  name: id
  type: string
- description: Event title displayed across all streaming platforms
  name: title
  type: string
- description: Event description
  name: description
  type: string
- description: Current status of the event
  name: status
  type: string
- description: ISO 8601 timestamp when the event started
  name: startedAt
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the event ended
  name: endedAt
  type:
  - string
  - 'null'
- description: List of channel IDs included in this event
  name: channels
  type: array
provider_name: Restream
provider_slug: restream
schema_file: json-schema/restream-event-schema.json
slug: restream-event
source_filename: restream-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.restream.io/schemas/event\",\n  \"title\": \"Event\",\n  \"description\": \"A Restream live streaming event, which can be scheduled, in-progress, or historical.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Event title displayed across all streaming platforms\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Event description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"upcoming\", \"in-progress\", \"completed\"],\n      \"description\": \"Current status of the event\"\n    },\n    \"startedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event started\"\
  \n    },\n    \"endedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event ended\"\n    },\n    \"channels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"List of channel IDs included in this event\"\n    }\n  },\n  \"required\": [\"id\", \"status\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/json-schema/restream-event-schema.json
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
title: Event
---
