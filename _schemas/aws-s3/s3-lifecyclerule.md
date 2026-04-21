---
description: A lifecycle rule for individual objects in an Amazon S3 bucket.
layout: schema
name: LifecycleRule
properties_list:
- description: ''
  name: Expiration
  type: object
- description: ''
  name: ID
  type: object
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Transitions
  type: object
- description: ''
  name: NoncurrentVersionTransitions
  type: object
- description: Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versio
  name: NoncurrentVersionExpiration
  type: object
- description: Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href="https://docs.
  name: AbortIncompleteMultipartUpload
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecyclerule-schema.json
slug: s3-lifecyclerule
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: LifecycleRule
---
