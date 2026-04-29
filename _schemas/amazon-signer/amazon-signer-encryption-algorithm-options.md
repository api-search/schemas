---
description: The encryption algorithm options that are available to a code signing job.
layout: schema
name: EncryptionAlgorithmOptions
properties_list:
- description: ''
  name: allowedValues
  type: object
- description: ''
  name: defaultValue
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-encryption-algorithm-options-schema.json
slug: amazon-signer-encryption-algorithm-options
source_filename: amazon-signer-encryption-algorithm-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-encryption-algorithm-options-schema.json\",\n  \"title\": \"EncryptionAlgorithmOptions\",\n  \"description\": \"The encryption algorithm options that are available to a code signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/EncryptionAlgorithm\"\n          }\n        },\n        {\n          \"description\": \"The set of accepted encryption algorithms that are allowed in a code signing job.\"\n        }\n      ]\n    },\n    \"defaultValue\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"RSA\",\n            \"ECDSA\"\n          ]\n        },\n        {\n          \"\
  description\": \"The default encryption algorithm that is used by a code signing job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"allowedValues\",\n    \"defaultValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-encryption-algorithm-options-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: EncryptionAlgorithmOptions
---
