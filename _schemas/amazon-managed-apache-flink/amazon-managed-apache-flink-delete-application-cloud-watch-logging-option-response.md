---
description: DeleteApplicationCloudWatchLoggingOptionResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationCloudWatchLoggingOptionResponse
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: CloudWatchLoggingOptionDescriptions
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-cloud-watch-logging-option-response-schema.json
slug: amazon-managed-apache-flink-delete-application-cloud-watch-logging-option-response
source_filename: amazon-managed-apache-flink-delete-application-cloud-watch-logging-option-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-cloud-watch-logging-option-response-schema.json\",\n  \"title\": \"DeleteApplicationCloudWatchLoggingOptionResponse\",\n  \"description\": \"DeleteApplicationCloudWatchLoggingOptionResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The application's Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The version ID of the application.\
  \ Kinesis Data Analytics updates the <code>ApplicationVersionId</code> each time you change the CloudWatch logging options.\"\n        }\n      ]\n    },\n    \"CloudWatchLoggingOptionDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLoggingOptionDescriptions\"\n        },\n        {\n          \"description\": \"The descriptions of the remaining CloudWatch logging options for the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-cloud-watch-logging-option-response-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationCloudWatchLoggingOptionResponse
---
