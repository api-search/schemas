---
description: Describes the Amazon Kinesis Data Firehose delivery stream that is configured as the streaming source in the application input configuration.
layout: schema
name: KinesisFirehoseInputDescription
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-kinesis-firehose-input-description-schema.json
slug: amazon-managed-apache-flink-kinesis-firehose-input-description
source_filename: amazon-managed-apache-flink-kinesis-firehose-input-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-firehose-input-description-schema.json\",\n  \"title\": \"KinesisFirehoseInputDescription\",\n  \"description\": \"Describes the Amazon Kinesis Data Firehose delivery stream that is configured as the streaming source in the application input configuration. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the delivery stream.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"<p>The ARN of the IAM role that Kinesis Data Analytics\
  \ assumes to access the stream.</p> <note> <p>Provided for backward compatibility. Applications that are created with the current API version have an application-level service execution role rather than a resource-level role.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-kinesis-firehose-input-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: KinesisFirehoseInputDescription
---
