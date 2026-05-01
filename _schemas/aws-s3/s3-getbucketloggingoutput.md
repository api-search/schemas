---
description: ''
layout: schema
name: GetBucketLoggingOutput
properties_list:
- description: Describes where logs are stored and the prefix that Amazon S3 assigns to all log object keys for a bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucket
  name: LoggingEnabled
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-getbucketloggingoutput-schema.json
slug: s3-getbucketloggingoutput
source_filename: s3-getbucketloggingoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetBucketLoggingOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoggingEnabled\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"TargetBucket\": {},\n        \"TargetGrants\": {},\n        \"TargetPrefix\": {}\n      },\n      \"required\": [\n        \"TargetBucket\",\n        \"TargetPrefix\"\n      ],\n      \"description\": \"Describes where logs are stored and the prefix that Amazon S3 assigns to all log object keys for a bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTlogging.html\\\">PUT Bucket logging</a> in the <i>Amazon S3 API Reference</i>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-getbucketloggingoutput-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: GetBucketLoggingOutput
---
