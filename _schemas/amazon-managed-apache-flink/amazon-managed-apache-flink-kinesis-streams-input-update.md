---
description: When you update the input configuration for a SQL-based Kinesis Data Analytics application, provides information about a Kinesis stream as the streaming source.
layout: schema
name: KinesisStreamsInputUpdate
properties_list:
- description: ''
  name: ResourceARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-kinesis-streams-input-update-schema.json
slug: amazon-managed-apache-flink-kinesis-streams-input-update
source_filename: amazon-managed-apache-flink-kinesis-streams-input-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-streams-input-update-schema.json\",\n  \"title\": \"KinesisStreamsInputUpdate\",\n  \"description\": \"When you update the input configuration for a SQL-based Kinesis Data Analytics application, provides information about a Kinesis stream as the streaming source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the input Kinesis data stream to read.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARNUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-streams-input-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: KinesisStreamsInputUpdate
---
