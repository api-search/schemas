---
description: Specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue when Amazon S3 detects specified events.
layout: schema
name: QueueConfiguration
properties_list:
- description: An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.
  name: Id
  type: string
- description: ''
  name: QueueArn
  type: object
- description: ''
  name: Events
  type: object
- description: Specifies object key name filtering rules. For information about key name filtering, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/NotificationHowTo.html">Configuring Event Notification
  name: Filter
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-queueconfiguration-schema.json
slug: s3-queueconfiguration
source_filename: s3-queueconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.\"\n    },\n    \"QueueArn\": {},\n    \"Events\": {},\n    \"Filter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Key\": {}\n      },\n      \"description\": \"Specifies object key name filtering rules. For information about key name filtering, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/NotificationHowTo.html\\\">Configuring Event Notifications</a> in the <i>Amazon S3 User Guide</i>.\"\n    }\n  },\n  \"required\": [\n    \"QueueArn\",\n    \"Events\"\n  ],\n  \"description\": \"Specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue\
  \ when Amazon S3 detects specified events.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-queueconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: QueueConfiguration
---
