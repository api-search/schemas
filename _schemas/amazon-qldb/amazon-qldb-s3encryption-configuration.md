---
description: The encryption settings that are used by a journal export job to write data in an Amazon Simple Storage Service (Amazon S3) bucket.
layout: schema
name: S3EncryptionConfiguration
properties_list:
- description: ''
  name: ObjectEncryptionType
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-s3encryption-configuration-schema.json
slug: amazon-qldb-s3encryption-configuration
source_filename: amazon-qldb-s3encryption-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-s3encryption-configuration-schema.json\",\n  \"title\": \"S3EncryptionConfiguration\",\n  \"description\": \"The encryption settings that are used by a journal export job to write data in an Amazon Simple Storage Service (Amazon S3) bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectEncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectEncryptionType\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 object encryption type.</p> <p>To learn more about server-side encryption options in Amazon S3, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\\\">Protecting Data Using Server-Side Encryption</a> in the <i>Amazon S3 Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n\
  \    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of a symmetric key in Key Management Service (KMS). Amazon S3 does not support asymmetric KMS keys.</p> <p>You must provide a <code>KmsKeyArn</code> if you specify <code>SSE_KMS</code> as the <code>ObjectEncryptionType</code>.</p> <p> <code>KmsKeyArn</code> is not required if you specify <code>SSE_S3</code> as the <code>ObjectEncryptionType</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ObjectEncryptionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-s3encryption-configuration-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: S3EncryptionConfiguration
---
