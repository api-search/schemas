---
description: ''
layout: schema
name: PutBucketNotificationConfigurationRequest
properties_list:
- description: A container for specifying the notification configuration of the bucket. If this element is empty, notifications are turned off for the bucket.
  name: NotificationConfiguration
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-putbucketnotificationconfigurationrequest-schema.json
slug: s3-putbucketnotificationconfigurationrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutBucketNotificationConfigurationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotificationConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"TopicConfigurations\": {},\n        \"QueueConfigurations\": {},\n        \"LambdaFunctionConfigurations\": {},\n        \"EventBridgeConfiguration\": {}\n      },\n      \"description\": \"A container for specifying the notification configuration of the bucket. If this element is empty, notifications are turned off for the bucket.\"\n    }\n  },\n  \"required\": [\n    \"NotificationConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-putbucketnotificationconfigurationrequest-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: PutBucketNotificationConfigurationRequest
---
