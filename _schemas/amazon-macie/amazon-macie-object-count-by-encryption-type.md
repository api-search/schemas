---
description: Provides information about the number of objects that are in an S3 bucket and use certain types of server-side encryption, use client-side encryption, or aren't encrypted.
layout: schema
name: ObjectCountByEncryptionType
properties_list:
- description: ''
  name: customerManaged
  type: object
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
schema_file: json-schema/amazon-macie-object-count-by-encryption-type-schema.json
slug: amazon-macie-object-count-by-encryption-type
source_filename: amazon-macie-object-count-by-encryption-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-object-count-by-encryption-type-schema.json\",\n  \"title\": \"ObjectCountByEncryptionType\",\n  \"description\": \"Provides information about the number of objects that are in an S3 bucket and use certain types of server-side encryption, use client-side encryption, or aren't encrypted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerManaged\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that are encrypted with a customer-provided key. The objects use customer-provided server-side encryption (SSE-C).\"\n        }\n      ]\n    },\n    \"kmsManaged\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n       \
  \ {\n          \"description\": \"The total number of objects that are encrypted with an KMS key, either an Amazon Web Services managed key or a customer managed key. The objects use KMS encryption (SSE-KMS).\"\n        }\n      ]\n    },\n    \"s3Managed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that are encrypted with an Amazon S3 managed key. The objects use Amazon S3 managed encryption (SSE-S3).\"\n        }\n      ]\n    },\n    \"unencrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that use client-side encryption or aren't encrypted.\"\n        }\n      ]\n    },\n    \"unknown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total\
  \ number of objects that Amazon Macie doesn't have current encryption metadata for. Macie can't provide current data about the encryption settings for these objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-object-count-by-encryption-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ObjectCountByEncryptionType
---
