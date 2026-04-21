---
description: A container for specifying the configuration for Lambda notifications.
layout: schema
name: LambdaFunctionConfiguration
properties_list:
- description: An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.
  name: Id
  type: string
- description: ''
  name: LambdaFunctionArn
  type: object
- description: ''
  name: Events
  type: object
- description: Specifies object key name filtering rules. For information about key name filtering, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/NotificationHowTo.html">Configuring Event Notification
  name: Filter
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lambdafunctionconfiguration-schema.json
slug: s3-lambdafunctionconfiguration
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: LambdaFunctionConfiguration
---
