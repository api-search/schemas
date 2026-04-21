---
description: Container for specifying the Lambda notification configuration.
layout: schema
name: CloudFunctionConfiguration
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
  name: CloudFunction
  type: object
- description: ''
  name: InvocationRole
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-cloudfunctionconfiguration-schema.json
slug: s3-cloudfunctionconfiguration
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CloudFunctionConfiguration
---
