---
description: Parameter information for generating a wrapped key using TR-31 or TR-34 standard.
layout: schema
name: WrappedKey
properties_list:
- description: ''
  name: KeyMaterial
  type: object
- description: ''
  name: WrappedKeyMaterialFormat
  type: object
- description: ''
  name: WrappingKeyArn
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-wrapped-key-schema.json
slug: openapi-wrapped-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-wrapped-key-schema.json\",\n  \"title\": \"WrappedKey\",\n  \"description\": \"Parameter information for generating a wrapped key using TR-31 or TR-34 standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyMaterial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyMaterial\"\n        },\n        {\n          \"description\": \"Parameter information for generating a wrapped key using TR-31 or TR-34 standard.\"\n        }\n      ]\n    },\n    \"WrappedKeyMaterialFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedKeyMaterialFormat\"\n        },\n        {\n          \"description\": \"The key block format of a wrapped key.\"\n        }\n      ]\n    },\n    \"WrappingKeyArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the wrapped key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyMaterial\",\n    \"WrappedKeyMaterialFormat\",\n    \"WrappingKeyArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-wrapped-key-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: WrappedKey
---
