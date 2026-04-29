---
description: The PublicAccessBlock configuration that you want to apply to this Amazon S3 bucket. You can enable the configuration options in any combination. For more information about when Amazon S3 considers a bucket or object public, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status">The Meaning of "Public"</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: PublicAccessBlockConfiguration
properties_list:
- description: ''
  name: BlockPublicAcls
  type: object
- description: ''
  name: IgnorePublicAcls
  type: object
- description: ''
  name: BlockPublicPolicy
  type: object
- description: ''
  name: RestrictPublicBuckets
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-publicaccessblockconfiguration-schema.json
slug: s3-publicaccessblockconfiguration
source_filename: s3-publicaccessblockconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublicAccessBlockConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockPublicAcls\": {},\n    \"IgnorePublicAcls\": {},\n    \"BlockPublicPolicy\": {},\n    \"RestrictPublicBuckets\": {}\n  },\n  \"description\": \"The PublicAccessBlock configuration that you want to apply to this Amazon S3 bucket. You can enable the configuration options in any combination. For more information about when Amazon S3 considers a bucket or object public, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html#access-control-block-public-access-policy-status\\\">The Meaning of \\\"Public\\\"</a> in the <i>Amazon S3 User Guide</i>. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-publicaccessblockconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: PublicAccessBlockConfiguration
---
