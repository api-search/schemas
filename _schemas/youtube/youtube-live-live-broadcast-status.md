---
description: Status information about a live broadcast including its privacy status and lifecycle status.
layout: schema
name: LiveBroadcastStatus
properties_list:
- description: The broadcast's status as it relates to the lifecycle of the broadcast.
  name: lifeCycleStatus
  type: string
- description: The broadcast's privacy status.
  name: privacyStatus
  type: string
- description: The broadcast's recording status.
  name: recordingStatus
  type: string
- description: Indicates whether the broadcast is designated as child-directed.
  name: madeForKids
  type: boolean
- description: Indicates whether the channel owner has designated the broadcast as being made for kids.
  name: selfDeclaredMadeForKids
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-broadcast-status-schema.json
slug: youtube-live-live-broadcast-status
source_filename: youtube-live-live-broadcast-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Status information about a live broadcast including its privacy status and lifecycle status.\",\n  \"properties\": {\n    \"lifeCycleStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The broadcast's status as it relates to the lifecycle of the broadcast.\",\n      \"example\": \"abandoned\",\n      \"enum\": [\n        \"abandoned\",\n        \"complete\",\n        \"completeStarting\",\n        \"created\",\n        \"live\",\n        \"liveStarting\",\n        \"ready\",\n        \"reclaimed\",\n        \"revoked\",\n        \"testStarting\",\n        \"testing\"\n      ]\n    },\n    \"privacyStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The broadcast's privacy status.\",\n      \"example\": \"private\",\n      \"enum\": [\n        \"private\",\n        \"public\",\n        \"unlisted\"\n      ]\n    },\n    \"recordingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The broadcast's recording status.\",\n      \"example\": \"notRecording\",\n      \"enum\": [\n        \"notRecording\",\n        \"recorded\",\n        \"recording\"\n      ]\n    },\n    \"madeForKids\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the broadcast is designated as child-directed.\",\n      \"example\": \"channel==UC_x5XG1OV2P6uZZ5FSM9Ttw\"\n    },\n    \"selfDeclaredMadeForKids\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the channel owner has designated the broadcast as being made for kids.\",\n      \"example\": \"channel==UC_x5XG1OV2P6uZZ5FSM9Ttw\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveBroadcastStatus\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-broadcast-status-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveBroadcastStatus
---
