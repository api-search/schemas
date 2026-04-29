---
description: Describes the default server-side encryption to apply to new objects in the bucket. If a PUT Object request doesn't specify any server-side encryption, this default encryption will be applied. If you don't specify a customer managed key at configuration, Amazon S3 automatically creates an Amazon Web Services KMS key in your Amazon Web Services account the first time that you add an object encrypted with SSE-KMS to a bucket. By default, Amazon S3 uses this KMS key for SSE-KMS. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTencryption.html">PUT Bucket encryption</a> in the <i>Amazon S3 API Reference</i>.
layout: schema
name: ServerSideEncryptionByDefault
properties_list:
- description: ''
  name: SSEAlgorithm
  type: object
- description: ''
  name: KMSMasterKeyID
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-serversideencryptionbydefault-schema.json
slug: s3-serversideencryptionbydefault
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerSideEncryptionByDefault\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SSEAlgorithm\": {},\n    \"KMSMasterKeyID\": {}\n  },\n  \"required\": [\n    \"SSEAlgorithm\"\n  ],\n  \"description\": \"Describes the default server-side encryption to apply to new objects in the bucket. If a PUT Object request doesn't specify any server-side encryption, this default encryption will be applied. If you don't specify a customer managed key at configuration, Amazon S3 automatically creates an Amazon Web Services KMS key in your Amazon Web Services account the first time that you add an object encrypted with SSE-KMS to a bucket. By default, Amazon S3 uses this KMS key for SSE-KMS. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTencryption.html\\\">PUT Bucket encryption</a> in the <i>Amazon S3 API Reference</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-serversideencryptionbydefault-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ServerSideEncryptionByDefault
---
