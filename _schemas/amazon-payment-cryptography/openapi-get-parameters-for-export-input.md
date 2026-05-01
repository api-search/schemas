---
description: GetParametersForExportInput schema from Amazon Payment Cryptography
layout: schema
name: GetParametersForExportInput
properties_list:
- description: ''
  name: KeyMaterialType
  type: object
- description: ''
  name: SigningKeyAlgorithm
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-parameters-for-export-input-schema.json
slug: openapi-get-parameters-for-export-input
source_filename: openapi-get-parameters-for-export-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-export-input-schema.json\",\n  \"title\": \"GetParametersForExportInput\",\n  \"description\": \"GetParametersForExportInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyMaterialType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyMaterialType\"\n        },\n        {\n          \"description\": \"The key block format type (for example, TR-34 or TR-31) to use during key material export. Export token is only required for a TR-34 key export, <code>TR34_KEY_BLOCK</code>. Export token is not required for TR-31 key export.\"\n        }\n      ]\n    },\n    \"SigningKeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAlgorithm\"\n       \
  \ },\n        {\n          \"description\": \"The signing key algorithm to generate a signing key certificate. This certificate signs the wrapped key under export within the TR-34 key block cryptogram. <code>RSA_2048</code> is the only signing key algorithm allowed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyMaterialType\",\n    \"SigningKeyAlgorithm\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-export-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetParametersForExportInput
---
