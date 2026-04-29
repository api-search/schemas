---
description: Describes the cross-origin access configuration for objects in an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/cors.html">Enabling Cross-Origin Resource Sharing</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: CORSConfiguration
properties_list:
- description: ''
  name: CORSRules
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-corsconfiguration-schema.json
slug: s3-corsconfiguration
source_filename: s3-corsconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CORSRules\": {}\n  },\n  \"required\": [\n    \"CORSRules\"\n  ],\n  \"description\": \"Describes the cross-origin access configuration for objects in an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/cors.html\\\">Enabling Cross-Origin Resource Sharing</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-corsconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CORSConfiguration
---
