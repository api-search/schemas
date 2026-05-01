---
description: An HTTP Live Streaming (HLS) encryption configuration.
layout: schema
name: HlsEncryption
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
  name: RepeatExtXKey
  type: object
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-hls-encryption-schema.json
slug: mediapackage-api-hls-encryption
source_filename: mediapackage-api-hls-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-encryption-schema.json\",\n  \"title\": \"HlsEncryption\",\n  \"description\": \"An HTTP Live Streaming (HLS) encryption configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConstantInitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantInitializationVector\"\n          },\n          \"description\": \"A constant initialization vector for encryption (optional).\\nWhen not specified the initialization vector will be periodically rotated.\\n\"\n        }\n      ]\n    },\n    \"EncryptionMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMethod\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"encryptionMethod\"\n          },\n          \"description\": \"The encryption method to use.\"\n        }\n      ]\n    },\n    \"KeyRotationIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyRotationIntervalSeconds\"\n          },\n          \"description\": \"Interval (in seconds) between each encryption key rotation.\"\n        }\n      ]\n    },\n    \"RepeatExtXKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"repeatExtXKey\"\n          },\n          \"description\": \"When enabled, the EXT-X-KEY tag will be repeated in output manifests.\"\n        }\n      ]\n    },\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpekeKeyProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-encryption-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsEncryption
---
