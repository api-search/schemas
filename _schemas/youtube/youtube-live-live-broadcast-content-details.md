---
description: Detailed settings for a live broadcast including stream configuration, DVR settings, and content configuration.
layout: schema
name: LiveBroadcastContentDetails
properties_list:
- description: The ID of the stream that is bound to the broadcast.
  name: boundStreamId
  type: string
- description: The date and time that the live stream referenced by boundStreamId was last updated.
  name: boundStreamLastUpdateTimeMs
  type: string
- description: The monitorStream object contains information about the monitor stream, which the broadcaster can use to review the event content before the broadcast stream is shown publicly.
  name: monitorStream
  type: object
- description: Indicates whether the broadcast video can be played in an embedded player.
  name: enableEmbed
  type: boolean
- description: Indicates whether the broadcast enables DVR controls. DVR controls enable the viewer to control the video playback experience by pausing, rewinding, or fast forwarding portions of the broadcast.
  name: enableDvr
  type: boolean
- description: Indicates whether YouTube should enable content encryption for the broadcast.
  name: enableContentEncryption
  type: boolean
- description: Indicates whether the broadcast should automatically begin with an in-stream slate when you update the broadcast's status to live.
  name: startWithSlate
  type: boolean
- description: Indicates whether the broadcast has captions enabled.
  name: closedCaptionsType
  type: string
- description: Indicates whether this broadcast has low latency enabled.
  name: enableLowLatency
  type: boolean
- description: Indicates latency preference for the broadcast. The options are ultraLow, low, and normal.
  name: latencyPreference
  type: string
- description: This setting indicates whether the broadcast should automatically begin streaming.
  name: enableAutoStart
  type: boolean
- description: Indicates whether the broadcast should automatically stop streaming.
  name: enableAutoStop
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-broadcast-content-details-schema.json
slug: youtube-live-live-broadcast-content-details
source_filename: youtube-live-live-broadcast-content-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed settings for a live broadcast including stream configuration, DVR settings, and content configuration.\",\n  \"properties\": {\n    \"boundStreamId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the stream that is bound to the broadcast.\",\n      \"example\": \"500123\"\n    },\n    \"boundStreamLastUpdateTimeMs\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the live stream referenced by boundStreamId was last updated.\",\n      \"example\": \"example_value\"\n    },\n    \"monitorStream\": {\n      \"type\": \"object\",\n      \"description\": \"The monitorStream object contains information about the monitor stream, which the broadcaster can use to review the event content before the broadcast stream is shown publicly.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"enableMonitorStream\": {\n          \"type\": \"boolean\",\n \
  \         \"description\": \"This value determines whether the monitor stream is enabled for the broadcast.\"\n        },\n        \"broadcastStreamDelayMs\": {\n          \"type\": \"integer\",\n          \"description\": \"If you have set the enableMonitorStream property to true, this value sets the delay between the video input and the broadcast monitor stream.\"\n        },\n        \"embedHtml\": {\n          \"type\": \"string\",\n          \"description\": \"The HTML code that embeds a player that plays the monitor stream.\"\n        }\n      }\n    },\n    \"enableEmbed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the broadcast video can be played in an embedded player.\",\n      \"example\": true\n    },\n    \"enableDvr\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the broadcast enables DVR controls. DVR controls enable the viewer to control the video playback experience by pausing, rewinding, or fast forwarding\
  \ portions of the broadcast.\",\n      \"example\": true\n    },\n    \"enableContentEncryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether YouTube should enable content encryption for the broadcast.\",\n      \"example\": true\n    },\n    \"startWithSlate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the broadcast should automatically begin with an in-stream slate when you update the broadcast's status to live.\",\n      \"example\": true\n    },\n    \"closedCaptionsType\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the broadcast has captions enabled.\",\n      \"example\": \"closedCaptionsDisabled\",\n      \"enum\": [\n        \"closedCaptionsDisabled\",\n        \"closedCaptionsEmbedded\",\n        \"closedCaptionsHttpPost\"\n      ]\n    },\n    \"enableLowLatency\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this broadcast has low latency enabled.\"\
  ,\n      \"example\": true\n    },\n    \"latencyPreference\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates latency preference for the broadcast. The options are ultraLow, low, and normal.\",\n      \"example\": \"low\",\n      \"enum\": [\n        \"low\",\n        \"normal\",\n        \"ultraLow\"\n      ]\n    },\n    \"enableAutoStart\": {\n      \"type\": \"boolean\",\n      \"description\": \"This setting indicates whether the broadcast should automatically begin streaming.\",\n      \"example\": true\n    },\n    \"enableAutoStop\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the broadcast should automatically stop streaming.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveBroadcastContentDetails\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-broadcast-content-details-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveBroadcastContentDetails
---
