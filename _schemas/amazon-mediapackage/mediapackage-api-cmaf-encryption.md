---
description: A Common Media Application Format (CMAF) encryption configuration.
layout: schema
name: CmafEncryption
properties_list:
- description: ''
  name: ConstantInitializationVector
  type: object
- description: ''
  name: EncryptionMethod
  type: object
- description: ''
  name: KeyRotationIntervalSeconds
  type: object
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-cmaf-encryption-schema.json
slug: mediapackage-api-cmaf-encryption
source_filename: mediapackage-api-cmaf-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-cmaf-encryption-schema.json\",\n  \"title\": \"CmafEncryption\",\n  \"description\": \"A Common Media Application Format (CMAF) encryption configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConstantInitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantInitializationVector\"\n          },\n          \"description\": \"An optional 128-bit, 16-byte hex value represented by a 32-character string, used in conjunction with the key for encrypting blocks. If you don't specify a value, then MediaPackage creates the constant initialization vector (IV).\"\n        }\n      ]\n    },\n    \"EncryptionMethod\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/CmafEncryptionMethod\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionMethod\"\n          }\n        }\n      ]\n    },\n    \"KeyRotationIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyRotationIntervalSeconds\"\n          },\n          \"description\": \"Time (in seconds) between each encryption key rotation.\"\n        }\n      ]\n    },\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpekeKeyProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-cmaf-encryption-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafEncryption
---
