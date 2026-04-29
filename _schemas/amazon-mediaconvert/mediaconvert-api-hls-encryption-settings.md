---
description: Settings for HLS encryption
layout: schema
name: HlsEncryptionSettings
properties_list:
- description: ''
  name: ConstantInitializationVector
  type: object
- description: ''
  name: EncryptionMethod
  type: object
- description: ''
  name: InitializationVectorInManifest
  type: object
- description: ''
  name: OfflineEncrypted
  type: object
- description: ''
  name: SpekeKeyProvider
  type: object
- description: ''
  name: StaticKeyProvider
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-encryption-settings-schema.json
slug: mediaconvert-api-hls-encryption-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-encryption-settings-schema.json\",\n  \"title\": \"HlsEncryptionSettings\",\n  \"description\": \"Settings for HLS encryption\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConstantInitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin32Max32Pattern09aFAF32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantInitializationVector\"\n          },\n          \"description\": \"This is a 128-bit, 16-byte hex value represented by a 32-character text string. If this parameter is not set then the Initialization Vector will follow the segment number by default.\"\n        }\n      ]\n    },\n    \"EncryptionMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsEncryptionType\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionMethod\"\n          },\n          \"description\": \"Encrypts the segments with the given encryption scheme. Leave blank to disable. Selecting 'Disabled' in the web interface also disables encryption.\"\n        }\n      ]\n    },\n    \"InitializationVectorInManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsInitializationVectorInManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"initializationVectorInManifest\"\n          },\n          \"description\": \"The Initialization Vector is a 128-bit number used in conjunction with the key for encrypting blocks. If set to INCLUDE, Initialization Vector is listed in the manifest. Otherwise Initialization Vector is not in the manifest.\"\n        }\n      ]\n    },\n    \"OfflineEncrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsOfflineEncrypted\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"offlineEncrypted\"\n          },\n          \"description\": \"Enable this setting to insert the EXT-X-SESSION-KEY element into the master playlist. This allows for offline Apple HLS FairPlay content protection.\"\n        }\n      ]\n    },\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          },\n          \"description\": \"If your output group type is HLS, DASH, or Microsoft Smooth, use these settings when doing DRM encryption with a SPEKE-compliant key provider. If your output group type is CMAF, use the SpekeKeyProviderCmaf settings instead.\"\n        }\n      ]\n    },\n    \"StaticKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticKeyProvider\"\n        },\n        {\n          \"xml\": {\n        \
  \    \"name\": \"staticKeyProvider\"\n          },\n          \"description\": \"Use these settings to set up encryption with a static key provider.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsKeyProviderType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Specify whether your DRM encryption key is static or from a key provider that follows the SPEKE standard. For more information about SPEKE, see https://docs.aws.amazon.com/speke/latest/documentation/what-is-speke.html.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-encryption-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsEncryptionSettings
---
