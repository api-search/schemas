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
tags:
- Broadcasting
- Live Streaming
- Media
- Streaming
- Video
- WebRTC
title: Broadcast
---
