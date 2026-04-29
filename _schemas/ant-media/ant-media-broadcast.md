---
description: An Ant Media Server broadcast/stream representing a live or recorded video stream with its configuration and current status.
layout: schema
name: Broadcast
properties_list:
- description: Unique identifier for the stream.
  name: streamId
  type: string
- description: Human-readable name for the broadcast.
  name: name
  type: string
- description: Current broadcast status.
  name: status
  type: string
- description: Type of broadcast.
  name: type
  type: string
- description: Protocol used to publish the stream.
  name: publishType
  type: string
- description: URL for RTSP, SRT, or IP camera source streams.
  name: streamUrl
  type: string
- description: Current number of HLS viewers.
  name: hlsViewerCount
  type: integer
- description: Current number of WebRTC viewers.
  name: webRTCViewerCount
  type: integer
- description: Current number of RTMP viewers.
  name: rtmpViewerCount
  type: integer
- description: Whether MP4 recording is enabled (1 = enabled, 0 = disabled).
  name: mp4Enabled
  type: integer
- description: Whether WebM recording is enabled.
  name: webMEnabled
  type: integer
- description: Duration of the stream in milliseconds.
  name: duration
  type: integer
- description: Unix epoch milliseconds when broadcasting started.
  name: startTime
  type: integer
- description: Absolute start time in Unix epoch milliseconds.
  name: absoluteStartTimeMs
  type: integer
- description: Planned start time in Unix epoch milliseconds for scheduled broadcasts.
  name: plannedStartDate
  type: integer
- description: Description of the broadcast.
  name: description
  type: string
- description: One-time publish token for secured stream publishing.
  name: token
  type: string
- description: Whether this is a 360-degree stream.
  name: is360
  type: boolean
- description: GPS latitude for geo-tagged streams.
  name: latitude
  type: string
- description: GPS longitude for geo-tagged streams.
  name: longitude
  type: string
- description: GPS altitude for geo-tagged streams.
  name: altitude
  type: string
provider_name: Ant Media
provider_slug: ant-media
schema_file: json-schema/ant-media-broadcast-schema.json
slug: ant-media-broadcast
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/json-schema/ant-media-broadcast-schema.json\",\n  \"title\": \"Broadcast\",\n  \"description\": \"An Ant Media Server broadcast/stream representing a live or recorded video stream with its configuration and current status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamId\": {\"type\": \"string\", \"description\": \"Unique identifier for the stream.\", \"example\": \"stream500123\"},\n    \"name\": {\"type\": \"string\", \"description\": \"Human-readable name for the broadcast.\", \"example\": \"Product Launch Livestream\"},\n    \"status\": {\"type\": \"string\", \"enum\": [\"created\", \"broadcasting\", \"finished\"], \"description\": \"Current broadcast status.\", \"example\": \"broadcasting\"},\n    \"type\": {\"type\": \"string\", \"enum\": [\"liveStream\", \"ipCamera\", \"streamSource\", \"VOD\"], \"\
  description\": \"Type of broadcast.\", \"example\": \"liveStream\"},\n    \"publishType\": {\"type\": \"string\", \"enum\": [\"WebRTC\", \"RTMP\", \"RTSP\", \"SRT\"], \"description\": \"Protocol used to publish the stream.\", \"example\": \"WebRTC\"},\n    \"streamUrl\": {\"type\": \"string\", \"format\": \"uri\", \"description\": \"URL for RTSP, SRT, or IP camera source streams.\", \"example\": \"rtsp://camera.example.com/stream\"},\n    \"hlsViewerCount\": {\"type\": \"integer\", \"description\": \"Current number of HLS viewers.\", \"example\": 1250},\n    \"webRTCViewerCount\": {\"type\": \"integer\", \"description\": \"Current number of WebRTC viewers.\", \"example\": 45},\n    \"rtmpViewerCount\": {\"type\": \"integer\", \"description\": \"Current number of RTMP viewers.\", \"example\": 0},\n    \"mp4Enabled\": {\"type\": \"integer\", \"description\": \"Whether MP4 recording is enabled (1 = enabled, 0 = disabled).\", \"example\": 1},\n    \"webMEnabled\": {\"type\": \"integer\", \"\
  description\": \"Whether WebM recording is enabled.\", \"example\": 0},\n    \"duration\": {\"type\": \"integer\", \"description\": \"Duration of the stream in milliseconds.\", \"example\": 300000},\n    \"startTime\": {\"type\": \"integer\", \"description\": \"Unix epoch milliseconds when broadcasting started.\", \"example\": 1745000000000},\n    \"absoluteStartTimeMs\": {\"type\": \"integer\", \"description\": \"Absolute start time in Unix epoch milliseconds.\", \"example\": 1745000000000},\n    \"plannedStartDate\": {\"type\": \"integer\", \"description\": \"Planned start time in Unix epoch milliseconds for scheduled broadcasts.\", \"example\": 1745000000000},\n    \"description\": {\"type\": \"string\", \"description\": \"Description of the broadcast.\", \"example\": \"Live product launch event with Q&A session.\"},\n    \"token\": {\"type\": \"string\", \"description\": \"One-time publish token for secured stream publishing.\", \"example\": \"abc123def456\"},\n    \"is360\": {\"type\"\
  : \"boolean\", \"description\": \"Whether this is a 360-degree stream.\", \"example\": false},\n    \"latitude\": {\"type\": \"string\", \"description\": \"GPS latitude for geo-tagged streams.\", \"example\": \"37.7749\"},\n    \"longitude\": {\"type\": \"string\", \"description\": \"GPS longitude for geo-tagged streams.\", \"example\": \"-122.4194\"},\n    \"altitude\": {\"type\": \"string\", \"description\": \"GPS altitude for geo-tagged streams.\", \"example\": \"10\"}\n  },\n  \"required\": [\"streamId\", \"name\", \"status\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/json-schema/ant-media-broadcast-schema.json
tags:
- Broadcasting
- Live Streaming
- Media
- Streaming
- Video
- WebRTC
title: Broadcast
---
