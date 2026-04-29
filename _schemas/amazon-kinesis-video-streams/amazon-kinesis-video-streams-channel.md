---
description: An Amazon Kinesis Video Streams signaling channel for WebRTC.
layout: schema
name: Channel
properties_list:
- description: The name of the signaling channel.
  name: ChannelName
  type: string
- description: The ARN of the signaling channel.
  name: ChannelARN
  type: string
- description: The type of the signaling channel.
  name: ChannelType
  type: string
- description: The status of the signaling channel.
  name: ChannelStatus
  type: string
- description: When the channel was created.
  name: CreationTime
  type: string
provider_name: Amazon Kinesis Video Streams
provider_slug: amazon-kinesis-video-streams
schema_file: json-schema/amazon-kinesis-video-streams-channel-schema.json
slug: amazon-kinesis-video-streams-channel
source_filename: amazon-kinesis-video-streams-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/json-schema/amazon-kinesis-video-streams-channel-schema.json\",\n  \"title\": \"Channel\",\n  \"description\": \"An Amazon Kinesis Video Streams signaling channel for WebRTC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the signaling channel.\",\n      \"example\": \"my-webrtc-channel\"\n    },\n    \"ChannelARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the signaling channel.\"\n    },\n    \"ChannelType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the signaling channel.\",\n      \"example\": \"SINGLE_MASTER\",\n      \"enum\": [\n        \"SINGLE_MASTER\",\n        \"FULL_MESH\"\n      ]\n    },\n    \"ChannelStatus\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The status of the signaling channel.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"UPDATING\",\n        \"DELETING\"\n      ]\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the channel was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/json-schema/amazon-kinesis-video-streams-channel-schema.json
tags:
- AWS
- IoT
- Machine Learning
- Media
- Video Streaming
title: Channel
---
