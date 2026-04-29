---
description: Specifies the lifecycle configuration for objects in an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/object-lifecycle-mgmt.html">Object Lifecycle Management</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: BucketLifecycleConfiguration
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-bucketlifecycleconfiguration-schema.json
slug: s3-bucketlifecycleconfiguration
source_filename: s3-bucketlifecycleconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BucketLifecycleConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {}\n  },\n  \"required\": [\n    \"Rules\"\n  ],\n  \"description\": \"Specifies the lifecycle configuration for objects in an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/object-lifecycle-mgmt.html\\\">Object Lifecycle Management</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-bucketlifecycleconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: BucketLifecycleConfiguration
---
