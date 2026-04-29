---
description: Use this structure to propose allowing <a href="https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations">cryptographic operations</a> in the grant only when the operation request includes the specified <a href="https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context">encryption context</a>. You can specify only one type of encryption context. An empty map is treated as not specified. For more information, see <a href="https://docs.aws.amazon.com/kms/latest/APIReference/API_GrantConstraints.html">GrantConstraints</a>.
layout: schema
name: KmsGrantConstraints
properties_list:
- description: ''
  name: encryptionContextEquals
  type: object
- description: ''
  name: encryptionContextSubset
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-kms-grant-constraints-schema.json
slug: iam-access-analyzer-kms-grant-constraints
source_filename: iam-access-analyzer-kms-grant-constraints-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-constraints-schema.json\",\n  \"title\": \"KmsGrantConstraints\",\n  \"description\": \"Use this structure to propose allowing <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\\\">cryptographic operations</a> in the grant only when the operation request includes the specified <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\\\">encryption context</a>. You can specify only one type of encryption context. An empty map is treated as not specified. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_GrantConstraints.html\\\">GrantConstraints</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionContextEquals\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsConstraintsMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that must match the encryption context in the <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\\\">cryptographic operation</a> request. The grant allows the operation only when the encryption context in the request is the same as the encryption context specified in this constraint.\"\n        }\n      ]\n    },\n    \"encryptionContextSubset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsConstraintsMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that must be included in the encryption context of the <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\\\">cryptographic operation</a> request. The grant allows the cryptographic operation\
  \ only when the encryption context in the request includes the key-value pairs specified in this constraint, although it can include additional key-value pairs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-kms-grant-constraints-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: KmsGrantConstraints
---
