---
description: An Amazon Kinesis data stream.
layout: schema
name: Stream
properties_list:
- description: The name of the stream.
  name: StreamName
  type: string
- description: The Amazon Resource Name (ARN) for the stream.
  name: StreamARN
  type: string
- description: The current status.
  name: StreamStatus
  type: string
- description: The current retention period, in hours.
  name: RetentionPeriodHours
  type: integer
- description: The approximate time the stream was created.
  name: StreamCreationTimestamp
  type: string
provider_name: Amazon Kinesis
provider_slug: amazon-kinesis
schema_file: json-schema/amazon-kinesis-stream-schema.json
slug: amazon-kinesis-stream
source_filename: amazon-kinesis-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/json-schema/amazon-kinesis-stream-schema.json\",\n  \"title\": \"Stream\",\n  \"description\": \"An Amazon Kinesis data stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stream.\",\n      \"example\": \"my-data-stream\"\n    },\n    \"StreamARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the stream.\"\n    },\n    \"StreamStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"CREATING\",\n        \"DELETING\",\n        \"ACTIVE\",\n        \"UPDATING\"\n      ]\n    },\n    \"RetentionPeriodHours\": {\n      \"type\": \"integer\",\n      \"description\": \"The current retention\
  \ period, in hours.\",\n      \"example\": 24\n    },\n    \"StreamCreationTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The approximate time the stream was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/json-schema/amazon-kinesis-stream-schema.json
tags:
- Analytics
- Big Data
- Data Processing
- Real-Time
- Streaming
title: Stream
---
