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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Rule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Expiration\": {},\n    \"ID\": {},\n    \"Prefix\": {},\n    \"Status\": {},\n    \"Transition\": {},\n    \"NoncurrentVersionTransition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"NoncurrentDays\": {},\n        \"StorageClass\": {},\n        \"NewerNoncurrentVersions\": {}\n      },\n      \"description\": \"Container for the transition rule that describes when noncurrent objects transition to the <code>STANDARD_IA</code>, <code>ONEZONE_IA</code>, <code>INTELLIGENT_TIERING</code>, <code>GLACIER_IR</code>, <code>GLACIER</code>, or <code>DEEP_ARCHIVE</code> storage class. If your bucket is versioning-enabled (or versioning is suspended), you can set this action to request that Amazon S3 transition noncurrent object versions to the <code>STANDARD_IA</code>, <code>ONEZONE_IA</code>, <code>INTELLIGENT_TIERING</code>,\
  \ <code>GLACIER_IR</code>, <code>GLACIER</code>, or <code>DEEP_ARCHIVE</code> storage class at a specific period in the object's lifetime.\"\n    },\n    \"NoncurrentVersionExpiration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"NoncurrentDays\": {},\n        \"NewerNoncurrentVersions\": {}\n      },\n      \"description\": \"Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versioning enabled (or suspended) to request that Amazon S3 delete noncurrent object versions at a specific period in the object's lifetime.\"\n    },\n    \"AbortIncompleteMultipartUpload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"DaysAfterInitiation\": {}\n      },\n      \"description\": \"Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts\
  \ of the upload. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/mpuoverview.html#mpu-abort-incomplete-mpu-lifecycle-config\\\"> Aborting Incomplete Multipart Uploads Using a Bucket Lifecycle Policy</a> in the <i>Amazon S3 User Guide</i>.\"\n    }\n  },\n  \"required\": [\n    \"Prefix\",\n    \"Status\"\n  ],\n  \"description\": \"Specifies lifecycle rules for an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTlifecycle.html\\\">Put Bucket Lifecycle Configuration</a> in the <i>Amazon S3 API Reference</i>. For examples, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketLifecycleConfiguration.html#API_PutBucketLifecycleConfiguration_Examples\\\">Put Bucket Lifecycle Configuration Examples</a>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-rule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Rule
---
