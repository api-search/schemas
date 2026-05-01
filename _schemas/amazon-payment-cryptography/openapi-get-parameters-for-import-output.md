---
description: GetParametersForImportOutput schema from Amazon Payment Cryptography
layout: schema
name: GetParametersForImportOutput
properties_list:
- description: ''
  name: ImportToken
  type: object
- description: ''
  name: ParametersValidUntilTimestamp
  type: object
- description: ''
  name: WrappingKeyAlgorithm
  type: object
- description: ''
  name: WrappingKeyCertificate
  type: object
- description: ''
  name: WrappingKeyCertificateChain
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-parameters-for-import-output-schema.json
slug: openapi-get-parameters-for-import-output
source_filename: openapi-get-parameters-for-import-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-import-output-schema.json\",\n  \"title\": \"GetParametersForImportOutput\",\n  \"description\": \"GetParametersForImportOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImportToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportTokenId\"\n        },\n        {\n          \"description\": \"The import token to initiate key import into Amazon Web Services Payment Cryptography. The import token expires after 7 days. You can use the same import token to import multiple keys to the same service account.\"\n        }\n      ]\n    },\n    \"ParametersValidUntilTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n   \
  \     {\n          \"description\": \"The validity period of the import token.\"\n        }\n      ]\n    },\n    \"WrappingKeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAlgorithm\"\n        },\n        {\n          \"description\": \"The algorithm of the wrapping key for use within TR-34 key block. <code>RSA_2048</code> is the only wrapping key algorithm allowed.\"\n        }\n      ]\n    },\n    \"WrappingKeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The wrapping key certificate of the wrapping key for use within the TR-34 key block. The certificate expires in 7 days.\"\n        }\n      ]\n    },\n    \"WrappingKeyCertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Payment Cryptography\
  \ certificate chain that signed the wrapping key certificate. This is the root certificate authority (CA) within your service account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ImportToken\",\n    \"ParametersValidUntilTimestamp\",\n    \"WrappingKeyAlgorithm\",\n    \"WrappingKeyCertificate\",\n    \"WrappingKeyCertificateChain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-import-output-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetParametersForImportOutput
---
