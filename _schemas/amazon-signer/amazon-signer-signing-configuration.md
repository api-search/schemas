---
description: The configuration of a code signing operation.
layout: schema
name: SigningConfiguration
properties_list:
- description: ''
  name: encryptionAlgorithmOptions
  type: object
- description: ''
  name: hashAlgorithmOptions
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-configuration-schema.json
slug: amazon-signer-signing-configuration
source_filename: amazon-signer-signing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-configuration-schema.json\",\n  \"title\": \"SigningConfiguration\",\n  \"description\": \"The configuration of a code signing operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionAlgorithmOptions\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"allowedValues\",\n            \"defaultValue\"\n          ],\n          \"properties\": {\n            \"allowedValues\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/EncryptionAlgorithms\"\n                },\n                {\n                  \"description\": \"The set of accepted encryption algorithms that are allowed in a code signing job.\"\n                }\n              ]\n            },\n\
  \            \"defaultValue\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/EncryptionAlgorithm\"\n                },\n                {\n                  \"description\": \"The default encryption algorithm that is used by a code signing job.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The encryption algorithm options that are available to a code signing job.\"\n        },\n        {\n          \"description\": \"The encryption algorithm options that are available for a code signing job.\"\n        }\n      ]\n    },\n    \"hashAlgorithmOptions\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"allowedValues\",\n            \"defaultValue\"\n          ],\n          \"properties\": {\n            \"allowedValues\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/HashAlgorithms\"\
  \n                },\n                {\n                  \"description\": \"The set of accepted hash algorithms allowed in a code signing job.\"\n                }\n              ]\n            },\n            \"defaultValue\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/HashAlgorithm\"\n                },\n                {\n                  \"description\": \"The default hash algorithm that is used in a code signing job.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The hash algorithms that are available to a code signing job.\"\n        },\n        {\n          \"description\": \"The hash algorithm options that are available for a code signing job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"encryptionAlgorithmOptions\",\n    \"hashAlgorithmOptions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-configuration-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningConfiguration
---
