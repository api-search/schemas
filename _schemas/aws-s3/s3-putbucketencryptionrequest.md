---
description: ''
layout: schema
name: PutBucketEncryptionRequest
properties_list:
- description: Specifies the default server-side-encryption configuration.
  name: ServerSideEncryptionConfiguration
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-putbucketencryptionrequest-schema.json
slug: s3-putbucketencryptionrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutBucketEncryptionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServerSideEncryptionConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Rules\": {}\n      },\n      \"required\": [\n        \"Rules\"\n      ],\n      \"description\": \"Specifies the default server-side-encryption configuration.\"\n    }\n  },\n  \"required\": [\n    \"ServerSideEncryptionConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-putbucketencryptionrequest-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: PutBucketEncryptionRequest
---
