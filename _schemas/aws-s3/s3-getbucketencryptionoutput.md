---
description: ''
layout: schema
name: GetBucketEncryptionOutput
properties_list:
- description: Specifies the default server-side-encryption configuration.
  name: ServerSideEncryptionConfiguration
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-getbucketencryptionoutput-schema.json
slug: s3-getbucketencryptionoutput
source_filename: s3-getbucketencryptionoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetBucketEncryptionOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServerSideEncryptionConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Rules\": {}\n      },\n      \"required\": [\n        \"Rules\"\n      ],\n      \"description\": \"Specifies the default server-side-encryption configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-getbucketencryptionoutput-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: GetBucketEncryptionOutput
---
