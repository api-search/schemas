---
description: An AWS KMS key (formerly customer master key) used for cryptographic operations.
layout: schema
name: Key
properties_list:
- description: The globally unique identifier for the KMS key.
  name: KeyId
  type: string
- description: The Amazon Resource Name (ARN) of the KMS key.
  name: KeyArn
  type: string
- description: The current status of the KMS key.
  name: KeyState
  type: string
- description: The cryptographic operations for which the KMS key can be used.
  name: KeyUsage
  type: string
- description: Describes the type of key material in the KMS key.
  name: KeySpec
  type: string
- description: The description of the KMS key.
  name: Description
  type: string
- description: The date and time when the KMS key was created.
  name: CreationDate
  type: string
- description: The date and time after which KMS deletes this KMS key.
  name: DeletionDate
  type: string
- description: Specifies whether the KMS key is enabled.
  name: Enabled
  type: boolean
- description: Indicates whether the KMS key is a multi-Region key.
  name: MultiRegion
  type: boolean
provider_name: Amazon KMS
provider_slug: amazon-kms
schema_file: json-schema/amazon-kms-key-schema.json
slug: amazon-kms-key
source_filename: amazon-kms-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kms/refs/heads/main/json-schema/amazon-kms-key-schema.json\",\n  \"title\": \"Key\",\n  \"description\": \"An AWS KMS key (formerly customer master key) used for cryptographic operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique identifier for the KMS key.\",\n      \"example\": \"mrk-1234abcd12ab34cd56ef1234567890ab\"\n    },\n    \"KeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the KMS key.\"\n    },\n    \"KeyState\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the KMS key.\",\n      \"example\": \"Enabled\",\n      \"enum\": [\n        \"Creating\",\n        \"Enabled\",\n        \"Disabled\",\n        \"PendingDeletion\",\n        \"PendingImport\"\
  ,\n        \"PendingReplicaDeletion\",\n        \"Unavailable\",\n        \"Updating\"\n      ]\n    },\n    \"KeyUsage\": {\n      \"type\": \"string\",\n      \"description\": \"The cryptographic operations for which the KMS key can be used.\",\n      \"example\": \"ENCRYPT_DECRYPT\",\n      \"enum\": [\n        \"SIGN_VERIFY\",\n        \"ENCRYPT_DECRYPT\",\n        \"GENERATE_VERIFY_MAC\"\n      ]\n    },\n    \"KeySpec\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the type of key material in the KMS key.\",\n      \"example\": \"SYMMETRIC_DEFAULT\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the KMS key.\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the KMS key was created.\",\n      \"format\": \"date-time\"\n    },\n    \"DeletionDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time after which KMS deletes\
  \ this KMS key.\",\n      \"format\": \"date-time\"\n    },\n    \"Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the KMS key is enabled.\"\n    },\n    \"MultiRegion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the KMS key is a multi-Region key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kms/refs/heads/main/json-schema/amazon-kms-key-schema.json
tags:
- Cryptography
- Data Protection
- Encryption
- Key Management
- Security
title: Key
---
