---
description: Describes the Amazon CloudWatch logging option.
layout: schema
name: CloudWatchLoggingOptionDescription
properties_list:
- description: ''
  name: CloudWatchLoggingOptionId
  type: object
- description: ''
  name: LogStreamARN
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-description-schema.json
slug: amazon-managed-apache-flink-cloud-watch-logging-option-description
source_filename: amazon-managed-apache-flink-cloud-watch-logging-option-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-description-schema.json\",\n  \"title\": \"CloudWatchLoggingOptionDescription\",\n  \"description\": \"Describes the Amazon CloudWatch logging option.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudWatchLoggingOptionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the CloudWatch logging option description.\"\n        }\n      ]\n    },\n    \"LogStreamARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogStreamARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the CloudWatch log to receive application messages.\"\n        }\n      ]\n    },\n    \"\
  RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"<p>The IAM ARN of the role to use to send application messages. </p> <note> <p>Provided for backward compatibility. Applications created with the current API version have an application-level service execution role rather than a resource-level role.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogStreamARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-cloud-watch-logging-option-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CloudWatchLoggingOptionDescription
---
