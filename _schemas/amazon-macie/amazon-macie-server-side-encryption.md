---
description: Provides information about the default server-side encryption settings for an S3 bucket or the encryption settings for an S3 object.
layout: schema
name: ServerSideEncryption
properties_list:
- description: ''
  name: encryptionType
  type: object
- description: ''
  name: kmsMasterKeyId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-server-side-encryption-schema.json
slug: amazon-macie-server-side-encryption
source_filename: amazon-macie-server-side-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-server-side-encryption-schema.json\",\n  \"title\": \"ServerSideEncryption\",\n  \"description\": \"Provides information about the default server-side encryption settings for an S3 bucket or the encryption settings for an S3 object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionType\"\n        },\n        {\n          \"description\": \"The server-side encryption algorithm that's used when storing data in the bucket or object. If default encryption settings aren't configured for the bucket or the object isn't encrypted using server-side encryption, this value is NONE.\"\n        }\n      ]\n    },\n    \"kmsMasterKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) or unique identifier (key ID) for the KMS key that's used to encrypt data in the bucket or the object. This value is null if an KMS key isn't used to encrypt the data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-server-side-encryption-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ServerSideEncryption
---
