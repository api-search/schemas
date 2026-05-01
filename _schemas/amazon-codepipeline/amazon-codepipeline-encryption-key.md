---
description: Represents information about the key used to encrypt data in the artifact store, such as an Amazon Web Services Key Management Service (Key Management Service) key.
layout: schema
name: EncryptionKey
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-encryption-key-schema.json
slug: amazon-codepipeline-encryption-key
source_filename: amazon-codepipeline-encryption-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-encryption-key-schema.json\",\n  \"title\": \"EncryptionKey\",\n  \"description\": \"Represents information about the key used to encrypt data in the artifact store, such as an Amazon Web Services Key Management Service (Key Management Service) key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyId\"\n        },\n        {\n          \"description\": \"<p>The ID used to identify the key. For an Amazon Web Services KMS key, you can use the key ID, the key ARN, or the alias ARN.</p> <note> <p>Aliases are recognized only in the account that created the KMS key. For cross-account actions, you can only use the key ID or key ARN to identify the key. Cross-account actions involve using\
  \ the role from the other account (AccountB), so specifying the key ID will use the key from the other account (AccountB).</p> </note>\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyType\"\n        },\n        {\n          \"description\": \"The type of encryption key, such as an Amazon Web Services KMS key. When creating or updating a pipeline, the value must be set to 'KMS'.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-encryption-key-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: EncryptionKey
---
