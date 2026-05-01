---
description: An Amazon Kinesis Video Stream.
layout: schema
name: Stream
properties_list:
- description: The name of the stream.
  name: StreamName
  type: string
- description: The Amazon Resource Name (ARN) of the stream.
  name: StreamARN
  type: string
- description: The status of the stream.
  name: Status
  type: string
- description: How long the channel retains data (in hours).
  name: DataRetentionInHours
  type: integer
- description: When the stream was created.
  name: CreationTime
  type: string
provider_name: Amazon Kinesis Video Streams
provider_slug: amazon-kinesis-video-streams
schema_file: json-schema/amazon-kinesis-video-streams-stream-schema.json
slug: amazon-kinesis-video-streams-stream
source_filename: amazon-kinesis-video-streams-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/json-schema/amazon-kinesis-video-streams-stream-schema.json\",\n  \"title\": \"Stream\",\n  \"description\": \"An Amazon Kinesis Video Stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stream.\",\n      \"example\": \"my-video-stream\"\n    },\n    \"StreamARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the stream.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the stream.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"UPDATING\",\n        \"DELETING\"\n      ]\n    },\n    \"DataRetentionInHours\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"How long the channel retains data (in hours).\",\n      \"example\": 24\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the stream was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-video-streams/refs/heads/main/json-schema/amazon-kinesis-video-streams-stream-schema.json
tags:
- IoT
- Machine Learning
- Media
- Video Streaming
title: Stream
---
