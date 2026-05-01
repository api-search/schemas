---
description: 'Use encryptionContractConfiguration to configure one or more content encryption keys for your endpoints that use SPEKE 2.0. The encryption contract defines which content keys are used to encrypt the audio and video tracks in your stream. To configure the encryption contract, specify which audio and video encryption presets to use. Note the following considerations when using encryptionContractConfiguration: encryptionContractConfiguration can be used for DASH or CMAF endpoints that use SPEKE 2.0. SPEKE 2.0 relies on the CPIX 2.3 specification. You must disable key rotation for this endpoint by setting keyRotationIntervalSeconds to 0.'
layout: schema
name: EncryptionContractConfiguration
properties_list:
- description: ''
  name: PresetSpeke20Audio
  type: object
- description: ''
  name: PresetSpeke20Video
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-encryption-contract-configuration-schema.json
slug: mediapackage-api-encryption-contract-configuration
source_filename: mediapackage-api-encryption-contract-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-encryption-contract-configuration-schema.json\",\n  \"title\": \"EncryptionContractConfiguration\",\n  \"description\": \"Use encryptionContractConfiguration to configure one or more content encryption keys for your endpoints that use SPEKE 2.0. \\nThe encryption contract defines which content keys are used to encrypt the audio and video tracks in your stream. \\nTo configure the encryption contract, specify which audio and video encryption presets to use.\\nNote the following considerations when using encryptionContractConfiguration:\\nencryptionContractConfiguration can be used for DASH or CMAF endpoints that use SPEKE 2.0. SPEKE 2.0 relies on the CPIX 2.3 specification.\\nYou must disable key rotation for this endpoint by setting keyRotationIntervalSeconds to 0.\\n\",\n  \"type\"\
  : \"object\",\n  \"properties\": {\n    \"PresetSpeke20Audio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetSpeke20Audio\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"presetSpeke20Audio\"\n          },\n          \"description\": \"A collection of audio encryption presets.\"\n        }\n      ]\n    },\n    \"PresetSpeke20Video\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetSpeke20Video\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"presetSpeke20Video\"\n          },\n          \"description\": \"A collection of video encryption presets.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PresetSpeke20Audio\",\n    \"PresetSpeke20Video\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-encryption-contract-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EncryptionContractConfiguration
---
