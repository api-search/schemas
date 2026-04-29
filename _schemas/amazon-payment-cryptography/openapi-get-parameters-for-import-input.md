---
description: GetParametersForImportInput schema from Amazon Payment Cryptography
layout: schema
name: GetParametersForImportInput
properties_list:
- description: ''
  name: KeyMaterialType
  type: object
- description: ''
  name: WrappingKeyAlgorithm
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-parameters-for-import-input-schema.json
slug: openapi-get-parameters-for-import-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-import-input-schema.json\",\n  \"title\": \"GetParametersForImportInput\",\n  \"description\": \"GetParametersForImportInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyMaterialType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyMaterialType\"\n        },\n        {\n          \"description\": \"The key block format type such as TR-34 or TR-31 to use during key material import. Import token is only required for TR-34 key import <code>TR34_KEY_BLOCK</code>. Import token is not required for TR-31 key import.\"\n        }\n      ]\n    },\n    \"WrappingKeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAlgorithm\"\n        },\n    \
  \    {\n          \"description\": \"The wrapping key algorithm to generate a wrapping key certificate. This certificate wraps the key under import within the TR-34 key block cryptogram. <code>RSA_2048</code> is the only wrapping key algorithm allowed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyMaterialType\",\n    \"WrappingKeyAlgorithm\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-import-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetParametersForImportInput
---
