---
description: Identifies a Kinesis data stream as the streaming source. You provide the stream's Amazon Resource Name (ARN).
layout: schema
name: KinesisStreamsInput
properties_list:
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-kinesis-streams-input-schema.json
slug: amazon-managed-apache-flink-kinesis-streams-input
source_filename: amazon-managed-apache-flink-kinesis-streams-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-streams-input-schema.json\",\n  \"title\": \"KinesisStreamsInput\",\n  \"description\": \" Identifies a Kinesis data stream as the streaming source. You provide the stream's Amazon Resource Name (ARN).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The ARN of the input Kinesis data stream to read.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-streams-input-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: KinesisStreamsInput
---
