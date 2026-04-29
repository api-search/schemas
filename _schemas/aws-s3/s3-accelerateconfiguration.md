---
description: Configures the transfer acceleration state for an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html">Amazon S3 Transfer Acceleration</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: AccelerateConfiguration
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-accelerateconfiguration-schema.json
slug: s3-accelerateconfiguration
source_filename: s3-accelerateconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccelerateConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"description\": \"Configures the transfer acceleration state for an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html\\\">Amazon S3 Transfer Acceleration</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-accelerateconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AccelerateConfiguration
---
