---
description: For a SQL-based Kinesis Data Analytics application, when updating an output configuration using the <a>UpdateApplication</a> operation, provides information about a Kinesis Data Firehose delivery stream that is configured as the destination.
layout: schema
name: KinesisFirehoseOutputUpdate
properties_list:
- description: ''
  name: ResourceARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-kinesis-firehose-output-update-schema.json
slug: amazon-managed-apache-flink-kinesis-firehose-output-update
source_filename: amazon-managed-apache-flink-kinesis-firehose-output-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-firehose-output-update-schema.json\",\n  \"title\": \"KinesisFirehoseOutputUpdate\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, when updating an output configuration using the <a>UpdateApplication</a> operation, provides information about a Kinesis Data Firehose delivery stream that is configured as the destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the delivery stream to write to. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARNUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-firehose-output-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: KinesisFirehoseOutputUpdate
---
