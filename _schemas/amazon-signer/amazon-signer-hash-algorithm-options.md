---
description: The hash algorithms that are available to a code signing job.
layout: schema
name: HashAlgorithmOptions
properties_list:
- description: ''
  name: allowedValues
  type: object
- description: ''
  name: defaultValue
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-hash-algorithm-options-schema.json
slug: amazon-signer-hash-algorithm-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-hash-algorithm-options-schema.json\",\n  \"title\": \"HashAlgorithmOptions\",\n  \"description\": \"The hash algorithms that are available to a code signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/HashAlgorithm\"\n          }\n        },\n        {\n          \"description\": \"The set of accepted hash algorithms allowed in a code signing job.\"\n        }\n      ]\n    },\n    \"defaultValue\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SHA1\",\n            \"SHA256\"\n          ]\n        },\n        {\n          \"description\": \"The default hash algorithm\
  \ that is used in a code signing job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"allowedValues\",\n    \"defaultValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-hash-algorithm-options-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: HashAlgorithmOptions
---
