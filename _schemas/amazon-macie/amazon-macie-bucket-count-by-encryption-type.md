---
description: Provides information about the number of S3 buckets whose settings do or don't specify default server-side encryption behavior for objects that are added to the buckets. For detailed information about these settings, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-encryption.html">Setting default server-side encryption behavior for Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.
layout: schema
name: BucketCountByEncryptionType
properties_list:
- description: ''
  name: kmsManaged
  type: object
- description: ''
  name: s3Managed
  type: object
- description: ''
  name: unencrypted
  type: object
- description: ''
  name: unknown
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-count-by-encryption-type-schema.json
slug: amazon-macie-bucket-count-by-encryption-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-encryption-type-schema.json\",\n  \"title\": \"BucketCountByEncryptionType\",\n  \"description\": \"Provides information about the number of S3 buckets whose settings do or don't specify default server-side encryption behavior for objects that are added to the buckets. For detailed information about these settings, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-encryption.html\\\">Setting default server-side encryption behavior for Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsManaged\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \" <p>The total number of buckets whose\
  \ default encryption settings are configured to encrypt new objects with an Amazon Web Services managed KMS key or a customer managed KMS key. By default, these buckets encrypt new objects automatically using SSE-KMS encryption.</p>\"\n        }\n      ]\n    },\n    \"s3Managed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets whose default encryption settings are configured to encrypt new objects with an Amazon S3 managed key. By default, these buckets encrypt new objects automatically using SSE-S3 encryption.\"\n        }\n      ]\n    },\n    \"unencrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that don't specify default server-side encryption behavior for new objects. Default encryption settings aren't configured for these buckets.\"\n\
  \        }\n      ]\n    },\n    \"unknown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that Amazon Macie doesn't have current encryption metadata for. Macie can't provide current data about the default encryption settings for these buckets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-encryption-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketCountByEncryptionType
---
