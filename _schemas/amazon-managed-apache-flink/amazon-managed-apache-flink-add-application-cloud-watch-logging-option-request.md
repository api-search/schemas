---
description: AddApplicationCloudWatchLoggingOptionRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationCloudWatchLoggingOptionRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: CloudWatchLoggingOption
  type: object
- description: ''
  name: ConditionalToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-cloud-watch-logging-option-request-schema.json
slug: amazon-managed-apache-flink-add-application-cloud-watch-logging-option-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-cloud-watch-logging-option-request-schema.json\",\n  \"title\": \"AddApplicationCloudWatchLoggingOptionRequest\",\n  \"description\": \"AddApplicationCloudWatchLoggingOptionRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The Kinesis Data Analytics application name.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The version ID of the Kinesis Data\
  \ Analytics application. You must provide the <code>CurrentApplicationVersionId</code> or the <code>ConditionalToken</code>.You can retrieve the application version ID using <a>DescribeApplication</a>. For better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    },\n    \"CloudWatchLoggingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLoggingOption\"\n        },\n        {\n          \"description\": \"Provides the Amazon CloudWatch log stream Amazon Resource Name (ARN). \"\n        }\n      ]\n    },\n    \"ConditionalToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionalToken\"\n        },\n        {\n          \"description\": \"A value you use to implement strong concurrency for application updates. You must provide the <code>CurrentApplicationVersionId</code> or the <code>ConditionalToken</code>.\
  \ You get the application's current <code>ConditionalToken</code> using <a>DescribeApplication</a>. For better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CloudWatchLoggingOption\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-cloud-watch-logging-option-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationCloudWatchLoggingOptionRequest
---
