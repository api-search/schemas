---
description: Provides information about the default server-side encryption settings for an S3 bucket. For detailed information about these settings, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-encryption.html">Setting default server-side encryption behavior for Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.
layout: schema
name: BucketServerSideEncryption
properties_list:
- description: ''
  name: kmsMasterKeyId
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-server-side-encryption-schema.json
slug: amazon-macie-bucket-server-side-encryption
source_filename: amazon-macie-bucket-server-side-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-server-side-encryption-schema.json\",\n  \"title\": \"BucketServerSideEncryption\",\n  \"description\": \"Provides information about the default server-side encryption settings for an S3 bucket. For detailed information about these settings, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-encryption.html\\\">Setting default server-side encryption behavior for Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsMasterKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) or unique identifier (key ID) for the KMS key that's used by default to encrypt objects\
  \ that are added to the bucket. This value is null if the bucket is configured to use an Amazon S3 managed key to encrypt new objects.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"description\": \"<p>The server-side encryption algorithm that's used by default to encrypt objects that are added to the bucket. Possible values are:</p> <ul><li><p>AES256 - New objects are encrypted with an Amazon S3 managed key. They use SSE-S3 encryption.</p></li> <li><p>aws:kms - New objects are encrypted with an KMS key (kmsMasterKeyId), either an Amazon Web Services managed key or a customer managed key. They use SSE-KMS encryption.</p></li> <li><p>NONE - The bucket's default encryption settings don't specify server-side encryption behavior for new objects.</p></li></ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-server-side-encryption-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketServerSideEncryption
---
