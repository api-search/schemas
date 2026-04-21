---
description: Specifies lifecycle rules for an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTlifecycle.html">Put Bucket Lifecycle Configuration</a> in the <i>Amazon S3 API Reference</i>. For examples, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketLifecycleConfiguration.html#API_PutBucketLifecycleConfiguration_Examples">Put Bucket Lifecycle Configuration Examples</a>.
layout: schema
name: Rule
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
  name: Status
  type: object
- description: ''
  name: Transition
  type: object
- description: Container for the transition rule that describes when noncurrent objects transition to the <code>STANDARD_IA</code>, <code>ONEZONE_IA</code>, <code>INTELLIGENT_TIERING</code>, <code>GLACIER_IR</code>,
  name: NoncurrentVersionTransition
  type: object
- description: Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versio
  name: NoncurrentVersionExpiration
  type: object
- description: Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href="https://docs.
  name: AbortIncompleteMultipartUpload
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-rule-schema.json
slug: s3-rule
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Rule
---
