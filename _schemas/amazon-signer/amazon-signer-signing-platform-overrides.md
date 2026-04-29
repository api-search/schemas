---
description: Any overrides that are applied to the signing configuration of a code signing platform.
layout: schema
name: SigningPlatformOverrides
properties_list:
- description: ''
  name: signingConfiguration
  type: object
- description: ''
  name: signingImageFormat
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-platform-overrides-schema.json
slug: amazon-signer-signing-platform-overrides
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-platform-overrides-schema.json\",\n  \"title\": \"SigningPlatformOverrides\",\n  \"description\": \"Any overrides that are applied to the signing configuration of a code signing platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"signingConfiguration\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"encryptionAlgorithm\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/EncryptionAlgorithm\"\n                },\n                {\n                  \"description\": \"A specified override of the default encryption algorithm that is used in a code signing job.\"\n                }\n              ]\n            },\n            \"hashAlgorithm\": {\n         \
  \     \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/HashAlgorithm\"\n                },\n                {\n                  \"description\": \"A specified override of the default hash algorithm that is used in a code signing job.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\"\n        },\n        {\n          \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\"\n        }\n      ]\n    },\n    \"signingImageFormat\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"JSON\",\n            \"JSONEmbedded\",\n            \"JSONDetached\"\n          ]\n        },\n        {\n          \"description\": \"A signed image is a JSON object. When overriding the default signing platform configuration,\
  \ a customer can select either of two signing formats, <code>JSONEmbedded</code> or <code>JSONDetached</code>. (A third format value, <code>JSON</code>, is reserved for future use.) With <code>JSONEmbedded</code>, the signing image has the payload embedded in it. With <code>JSONDetached</code>, the payload is not be embedded in the signing image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-platform-overrides-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningPlatformOverrides
---
