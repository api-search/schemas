---
description: ''
layout: schema
name: LifecycleRules
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-lifecyclerules-schema.json
slug: s3-lifecyclerules
source_filename: s3-lifecyclerules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleRules\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Expiration\": {},\n      \"ID\": {},\n      \"Prefix\": {},\n      \"Filter\": {},\n      \"Status\": {},\n      \"Transitions\": {},\n      \"NoncurrentVersionTransitions\": {},\n      \"NoncurrentVersionExpiration\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"NoncurrentDays\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/Days\"\n              },\n              {\n                \"description\": \"Specifies the number of days an object is noncurrent before Amazon S3 can perform the associated action. The value must be a non-zero positive integer. For information about the noncurrent days calculations, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/intro-lifecycle-rules.html#non-current-days-calculations\\\
  \">How Amazon S3 Calculates When an Object Became Noncurrent</a> in the <i>Amazon S3 User Guide</i>.\"\n              }\n            ]\n          },\n          \"NewerNoncurrentVersions\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/VersionCount\"\n              },\n              {\n                \"description\": \"Specifies how many noncurrent versions Amazon S3 will retain. If there are this many more recent noncurrent versions, Amazon S3 will take the associated action. For more information about noncurrent versions, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/intro-lifecycle-rules.html\\\">Lifecycle configuration elements</a> in the <i>Amazon S3 User Guide</i>.\"\n              }\n            ]\n          }\n        },\n        \"description\": \"Specifies when noncurrent object versions expire. Upon expiration, Amazon S3 permanently deletes the noncurrent object versions. You set this lifecycle configuration\
  \ action on a bucket that has versioning enabled (or suspended) to request that Amazon S3 delete noncurrent object versions at a specific period in the object's lifetime.\"\n      },\n      \"AbortIncompleteMultipartUpload\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DaysAfterInitiation\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/DaysAfterInitiation\"\n              },\n              {\n                \"description\": \"Specifies the number of days after which Amazon S3 aborts an incomplete multipart upload.\"\n              }\n            ]\n          }\n        },\n        \"description\": \"Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/mpuoverview.html#mpu-abort-incomplete-mpu-lifecycle-config\\\"> Aborting Incomplete\
  \ Multipart Uploads Using a Bucket Lifecycle Policy</a> in the <i>Amazon S3 User Guide</i>.\"\n      }\n    },\n    \"required\": [\n      \"Status\"\n    ],\n    \"description\": \"A lifecycle rule for individual objects in an Amazon S3 bucket.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-lifecyclerules-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: LifecycleRules
---
