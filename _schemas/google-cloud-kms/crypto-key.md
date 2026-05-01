---
description: A Google Cloud KMS cryptographic key resource used for encryption, decryption, signing, or verification operations.
layout: schema
name: CryptoKey
properties_list:
- description: Resource name of the crypto key.
  name: name
  type: string
- description: The primary version of the crypto key.
  name: primary
  type: object
- description: Immutable purpose of the crypto key.
  name: purpose
  type: string
- description: Timestamp when the key was created.
  name: createTime
  type: string
- description: Timestamp of the next scheduled key rotation.
  name: nextRotationTime
  type: string
- description: Rotation period of the key in seconds format.
  name: rotationPeriod
  type: string
- description: Template describing settings for new crypto key versions.
  name: versionTemplate
  type: object
- description: Duration before scheduled destruction completes.
  name: destroyScheduledDuration
  type: string
- description: Labels applied to the crypto key.
  name: labels
  type: object
- description: Whether this key may contain imported versions only.
  name: importOnly
  type: boolean
provider_name: Google Cloud KMS
provider_slug: google-cloud-kms
schema_file: json-schema/crypto-key.json
slug: crypto-key
source_filename: crypto-key.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-kms/refs/heads/main/json-schema/crypto-key.json\",\n  \"title\": \"CryptoKey\",\n  \"description\": \"A Google Cloud KMS cryptographic key resource used for encryption, decryption, signing, or verification operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the crypto key.\"\n    },\n    \"primary\": {\n      \"type\": \"object\",\n      \"description\": \"The primary version of the crypto key.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the crypto key version.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"CRYPTO_KEY_VERSION_STATE_UNSPECIFIED\",\n            \"PENDING_GENERATION\",\n         \
  \   \"ENABLED\",\n            \"DISABLED\",\n            \"DESTROYED\",\n            \"DESTROY_SCHEDULED\",\n            \"PENDING_IMPORT\",\n            \"IMPORT_FAILED\"\n          ],\n          \"description\": \"Current state of the key version.\"\n        },\n        \"protectionLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"PROTECTION_LEVEL_UNSPECIFIED\", \"SOFTWARE\", \"HSM\", \"EXTERNAL\", \"EXTERNAL_VPC\"],\n          \"description\": \"Protection level of the key version.\"\n        },\n        \"algorithm\": {\n          \"type\": \"string\",\n          \"description\": \"Algorithm of the key version.\"\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the version was created.\"\n        },\n        \"generateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the key material was\
  \ generated.\"\n        }\n      }\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CRYPTO_KEY_PURPOSE_UNSPECIFIED\",\n        \"ENCRYPT_DECRYPT\",\n        \"ASYMMETRIC_SIGN\",\n        \"ASYMMETRIC_DECRYPT\",\n        \"MAC\"\n      ],\n      \"description\": \"Immutable purpose of the crypto key.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the key was created.\"\n    },\n    \"nextRotationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the next scheduled key rotation.\"\n    },\n    \"rotationPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"Rotation period of the key in seconds format.\"\n    },\n    \"versionTemplate\": {\n      \"type\": \"object\",\n      \"description\": \"Template describing settings for new crypto key versions.\",\n      \"properties\": {\n        \"\
  protectionLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"PROTECTION_LEVEL_UNSPECIFIED\", \"SOFTWARE\", \"HSM\", \"EXTERNAL\", \"EXTERNAL_VPC\"]\n        },\n        \"algorithm\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"destroyScheduledDuration\": {\n      \"type\": \"string\",\n      \"description\": \"Duration before scheduled destruction completes.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels applied to the crypto key.\"\n    },\n    \"importOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this key may contain imported versions only.\"\n    }\n  },\n  \"required\": [\"purpose\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-kms/refs/heads/main/json-schema/crypto-key.json
tags:
- Cryptography
- Encryption
- Google Cloud
- Key Management
- KMS
- Security
title: CryptoKey
---
