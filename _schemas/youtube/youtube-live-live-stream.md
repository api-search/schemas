---
description: A liveStream resource contains information about the video stream that you are transmitting to YouTube. The stream provides the content that will be broadcast to YouTube users.
layout: schema
name: LiveStream
properties_list:
- description: Identifies the API resource's type. Value is youtube#liveStream.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube assigns to uniquely identify the stream.
  name: id
  type: string
- description: Basic details about a live stream including its title, description, and channel association.
  name: snippet
  type: object
- description: The cdn object defines the live stream's content delivery network (CDN) settings.
  name: cdn
  type: object
- description: Status information about a live stream including its stream status and health status.
  name: status
  type: object
- description: Detailed settings for a live stream including the stream key and ingestion settings.
  name: contentDetails
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-stream-schema.json
slug: youtube-live-live-stream
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A liveStream resource contains information about the video stream that you are transmitting to YouTube. The stream provides the content that will be broadcast to YouTube users.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#liveStream.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube assigns to uniquely identify the stream.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"Basic details about a live stream including its title, description, and channel association.\",\n      \"properties\": {\n        \"channelId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The ID of the channel to which this stream is affiliated.\",\n          \"example\": \"500123\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The stream's title. The value must be between 1 and 128 characters long.\",\n          \"example\": \"Example Title\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The stream's description. The value cannot be longer than 10000 characters.\",\n          \"example\": \"A sample description for this resource.\"\n        },\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time that the stream was created.\",\n          \"example\": \"2026-01-15T10:30:00Z\",\n          \"format\": \"date-time\"\n        },\n        \"isDefaultStream\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether this stream\
  \ is the default stream.\",\n          \"example\": true\n        }\n      }\n    },\n    \"cdn\": {\n      \"type\": \"object\",\n      \"description\": \"The cdn object defines the live stream's content delivery network (CDN) settings.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"ingestionType\": {\n          \"type\": \"string\",\n          \"description\": \"The method or protocol used to transmit the video stream.\",\n          \"enum\": [\n            \"dash\",\n            \"rtmp\",\n            \"webrtc\"\n          ]\n        },\n        \"ingestionInfo\": {\n          \"type\": \"object\",\n          \"description\": \"The ingestionInfo object contains information that YouTube provides that you need to transmit your RTMP or HTTP stream to YouTube.\",\n          \"properties\": {\n            \"streamName\": {\n              \"type\": \"string\",\n              \"description\": \"The stream name that YouTube assigns to the video stream.\"\n   \
  \         },\n            \"ingestionAddress\": {\n              \"type\": \"string\",\n              \"description\": \"The primary ingestion URL that you should use to stream video to YouTube.\"\n            },\n            \"backupIngestionAddress\": {\n              \"type\": \"string\",\n              \"description\": \"The backup ingestion URL that you should use to stream video to YouTube.\"\n            },\n            \"rtmpsIngestionAddress\": {\n              \"type\": \"string\",\n              \"description\": \"The primary secured ingestion URL that you should use to stream video to YouTube.\"\n            },\n            \"backupRtmpsIngestionAddress\": {\n              \"type\": \"string\",\n              \"description\": \"The backup secured ingestion URL that you should use to stream video to YouTube.\"\n            }\n          }\n        },\n        \"resolution\": {\n          \"type\": \"string\",\n          \"description\": \"The resolution of the inbound video data.\"\
  \n        },\n        \"frameRate\": {\n          \"type\": \"string\",\n          \"description\": \"The frame rate of the inbound video data.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"Status information about a live stream including its stream status and health status.\",\n      \"properties\": {\n        \"streamStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The stream's current status.\",\n          \"example\": \"active\",\n          \"enum\": [\n            \"active\",\n            \"created\",\n            \"error\",\n            \"inactive\",\n            \"ready\"\n          ]\n        },\n        \"healthStatus\": {\n          \"type\": \"object\",\n          \"description\": \"The health status of the stream.\",\n          \"example\": \"example_value\",\n          \"properties\": {\n            \"status\": {\n              \"type\": \"string\",\n              \"description\": \"The status\
  \ code of this stream.\",\n              \"enum\": [\n                \"bad\",\n                \"good\",\n                \"noData\",\n                \"ok\",\n                \"revoked\"\n              ]\n            },\n            \"lastUpdateTimeSeconds\": {\n              \"type\": \"integer\",\n              \"description\": \"The last time this status was updated, as a Unix timestamp.\",\n              \"format\": \"int64\"\n            },\n            \"configurationIssues\": {\n              \"type\": \"array\",\n              \"description\": \"The configurations issues on this stream.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"description\": \"The kind of error happening.\"\n                  },\n                  \"severity\": {\n                    \"type\": \"string\",\n                    \"description\": \"How severe\
  \ this issue is to the stream.\",\n                    \"enum\": [\n                      \"error\",\n                      \"info\",\n                      \"warning\"\n                    ]\n                  },\n                  \"reason\": {\n                    \"type\": \"string\",\n                    \"description\": \"The short-form reason for this issue.\"\n                  },\n                  \"description\": {\n                    \"type\": \"string\",\n                    \"description\": \"The long-form description of the issue and how to resolve it.\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"contentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed settings for a live stream including the stream key and ingestion settings.\",\n      \"properties\": {\n        \"boundBroadcastId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the live\
  \ broadcast to which this stream is bound.\",\n          \"example\": \"500123\"\n        },\n        \"isReusable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the stream is reusable, which means that it can be bound to multiple broadcasts.\",\n          \"example\": true\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveStream\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-stream-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveStream
---
