---
description: Describes the Amazon CloudWatch logging option updates.
layout: schema
name: CloudWatchLoggingOptionUpdate
properties_list:
- description: ''
  name: CloudWatchLoggingOptionId
  type: object
- description: ''
  name: LogStreamARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-update-schema.json
slug: amazon-managed-apache-flink-cloud-watch-logging-option-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-update-schema.json\",\n  \"title\": \"CloudWatchLoggingOptionUpdate\",\n  \"description\": \"Describes the Amazon CloudWatch logging option updates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudWatchLoggingOptionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the CloudWatch logging option to update\"\n        }\n      ]\n    },\n    \"LogStreamARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogStreamARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the CloudWatch log to receive application messages.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"CloudWatchLoggingOptionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CloudWatchLoggingOptionUpdate
---
