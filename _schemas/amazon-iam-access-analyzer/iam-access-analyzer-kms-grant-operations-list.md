---
description: KmsGrantOperationsList schema from AWS IAM Access Analyzer API
layout: schema
name: KmsGrantOperationsList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-kms-grant-operations-list-schema.json
slug: iam-access-analyzer-kms-grant-operations-list
source_filename: iam-access-analyzer-kms-grant-operations-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-operations-list-schema.json\",\n  \"title\": \"KmsGrantOperationsList\",\n  \"description\": \"KmsGrantOperationsList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"CreateGrant\",\n      \"Decrypt\",\n      \"DescribeKey\",\n      \"Encrypt\",\n      \"GenerateDataKey\",\n      \"GenerateDataKeyPair\",\n      \"GenerateDataKeyPairWithoutPlaintext\",\n      \"GenerateDataKeyWithoutPlaintext\",\n      \"GetPublicKey\",\n      \"ReEncryptFrom\",\n      \"ReEncryptTo\",\n      \"RetireGrant\",\n      \"Sign\",\n      \"Verify\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-operations-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: KmsGrantOperationsList
---
