---
description: A container for specifying the notification configuration of the bucket. If this element is empty, notifications are turned off for the bucket.
layout: schema
name: NotificationConfiguration
properties_list:
- description: ''
  name: TopicConfigurations
  type: object
- description: ''
  name: QueueConfigurations
  type: object
- description: ''
  name: LambdaFunctionConfigurations
  type: object
- description: ''
  name: EventBridgeConfiguration
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-notificationconfiguration-schema.json
slug: s3-notificationconfiguration
source_filename: s3-notificationconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TopicConfigurations\": {},\n    \"QueueConfigurations\": {},\n    \"LambdaFunctionConfigurations\": {},\n    \"EventBridgeConfiguration\": {}\n  },\n  \"description\": \"A container for specifying the notification configuration of the bucket. If this element is empty, notifications are turned off for the bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-notificationconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: NotificationConfiguration
---
