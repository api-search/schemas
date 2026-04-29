---
description: Provides a description of Amazon CloudWatch logging options, including the log stream Amazon Resource Name (ARN).
layout: schema
name: CloudWatchLoggingOption
properties_list:
- description: ''
  name: LogStreamARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-schema.json
slug: amazon-managed-apache-flink-cloud-watch-logging-option
source_filename: amazon-managed-apache-flink-cloud-watch-logging-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-schema.json\",\n  \"title\": \"CloudWatchLoggingOption\",\n  \"description\": \"Provides a description of Amazon CloudWatch logging options, including the log stream Amazon Resource Name (ARN). \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogStreamARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogStreamARN\"\n        },\n        {\n          \"description\": \"The ARN of the CloudWatch log to receive application messages.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogStreamARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CloudWatchLoggingOption
---
