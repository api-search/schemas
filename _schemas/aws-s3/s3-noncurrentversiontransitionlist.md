---
description: ''
layout: schema
name: NoncurrentVersionTransitionList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-noncurrentversiontransitionlist-schema.json
slug: s3-noncurrentversiontransitionlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoncurrentVersionTransitionList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"NoncurrentDays\": {},\n      \"StorageClass\": {},\n      \"NewerNoncurrentVersions\": {}\n    },\n    \"description\": \"Container for the transition rule that describes when noncurrent objects transition to the <code>STANDARD_IA</code>, <code>ONEZONE_IA</code>, <code>INTELLIGENT_TIERING</code>, <code>GLACIER_IR</code>, <code>GLACIER</code>, or <code>DEEP_ARCHIVE</code> storage class. If your bucket is versioning-enabled (or versioning is suspended), you can set this action to request that Amazon S3 transition noncurrent object versions to the <code>STANDARD_IA</code>, <code>ONEZONE_IA</code>, <code>INTELLIGENT_TIERING</code>, <code>GLACIER_IR</code>, <code>GLACIER</code>, or <code>DEEP_ARCHIVE</code> storage class at a specific period in the object's lifetime.\"\
  \n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-noncurrentversiontransitionlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: NoncurrentVersionTransitionList
---
