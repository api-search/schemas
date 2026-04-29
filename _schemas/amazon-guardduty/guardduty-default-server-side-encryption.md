---
description: Contains information on the server side encryption method used in the S3 bucket. See <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html">S3 Server-Side Encryption</a> for more information.
layout: schema
name: DefaultServerSideEncryption
properties_list:
- description: ''
  name: EncryptionType
  type: object
- description: ''
  name: KmsMasterKeyArn
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-default-server-side-encryption-schema.json
slug: guardduty-default-server-side-encryption
source_filename: guardduty-default-server-side-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-default-server-side-encryption-schema.json\",\n  \"title\": \"DefaultServerSideEncryption\",\n  \"description\": \"Contains information on the server side encryption method used in the S3 bucket. See <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\\\">S3 Server-Side Encryption</a> for more information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionType\"\n          },\n          \"description\": \"The type of encryption used for objects within the S3 bucket.\"\n        }\n      ]\n    },\n    \"KmsMasterKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsMasterKeyArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the KMS encryption key. Only available if the bucket <code>EncryptionType</code> is <code>aws:kms</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-default-server-side-encryption-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DefaultServerSideEncryption
---
