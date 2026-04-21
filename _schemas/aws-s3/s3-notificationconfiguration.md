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
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: NotificationConfiguration
---
