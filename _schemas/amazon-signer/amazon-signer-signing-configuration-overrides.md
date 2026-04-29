---
description: A signing configuration that overrides the default encryption or hash algorithm of a signing job.
layout: schema
name: SigningConfigurationOverrides
properties_list:
- description: ''
  name: encryptionAlgorithm
  type: object
- description: ''
  name: hashAlgorithm
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-configuration-overrides-schema.json
slug: amazon-signer-signing-configuration-overrides
source_filename: amazon-signer-signing-configuration-overrides-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-configuration-overrides-schema.json\",\n  \"title\": \"SigningConfigurationOverrides\",\n  \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionAlgorithm\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"RSA\",\n            \"ECDSA\"\n          ]\n        },\n        {\n          \"description\": \"A specified override of the default encryption algorithm that is used in a code signing job.\"\n        }\n      ]\n    },\n    \"hashAlgorithm\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SHA1\",\n            \"SHA256\"\n          ]\n        },\n\
  \        {\n          \"description\": \"A specified override of the default hash algorithm that is used in a code signing job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-configuration-overrides-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningConfigurationOverrides
---
