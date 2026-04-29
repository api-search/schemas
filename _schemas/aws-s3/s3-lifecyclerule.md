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
source_filename: s3-lifecyclerule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Expiration\": {},\n    \"ID\": {},\n    \"Prefix\": {},\n    \"Filter\": {},\n    \"Status\": {},\n    \"Transitions\": {},\n    \"NoncurrentVersionTransitions\": {},\n    \"NoncurrentVersionExpiration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"NoncurrentDays\": {},\n        \"NewerNoncurrentVersions\": {}\n      },\n      \"description\": \"Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration action on a bucket that has versioning enabled (or suspended) to request that Amazon S3 delete noncurrent object versions at a specific period in the object's lifetime.\"\n    },\n    \"AbortIncompleteMultipartUpload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"DaysAfterInitiation\"\
  : {}\n      },\n      \"description\": \"Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/mpuoverview.html#mpu-abort-incomplete-mpu-lifecycle-config\\\"> Aborting Incomplete Multipart Uploads Using a Bucket Lifecycle Policy</a> in the <i>Amazon S3 User Guide</i>.\"\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ],\n  \"description\": \"A lifecycle rule for individual objects in an Amazon S3 bucket.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecyclerule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: LifecycleRule
---
