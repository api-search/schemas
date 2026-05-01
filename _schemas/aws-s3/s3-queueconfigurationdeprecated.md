---
description: This data type is deprecated. Use <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_QueueConfiguration.html">QueueConfiguration</a> for the same purposes. This data type specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue when Amazon S3 detects specified events.
layout: schema
name: QueueConfigurationDeprecated
properties_list:
- description: An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.
  name: Id
  type: string
- description: ''
  name: Event
  type: object
- description: ''
  name: Events
  type: object
- description: ''
  name: Queue
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-queueconfigurationdeprecated-schema.json
slug: s3-queueconfigurationdeprecated
source_filename: s3-queueconfigurationdeprecated-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueConfigurationDeprecated\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.\"\n    },\n    \"Event\": {},\n    \"Events\": {},\n    \"Queue\": {}\n  },\n  \"description\": \"This data type is deprecated. Use <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_QueueConfiguration.html\\\">QueueConfiguration</a> for the same purposes. This data type specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue when Amazon S3 detects specified events. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-queueconfigurationdeprecated-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: QueueConfigurationDeprecated
---
