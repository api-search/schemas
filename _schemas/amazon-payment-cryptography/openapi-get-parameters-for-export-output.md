---
description: GetParametersForExportOutput schema from Amazon Payment Cryptography
layout: schema
name: GetParametersForExportOutput
properties_list:
- description: ''
  name: ExportToken
  type: object
- description: ''
  name: ParametersValidUntilTimestamp
  type: object
- description: ''
  name: SigningKeyAlgorithm
  type: object
- description: ''
  name: SigningKeyCertificate
  type: object
- description: ''
  name: SigningKeyCertificateChain
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-parameters-for-export-output-schema.json
slug: openapi-get-parameters-for-export-output
source_filename: openapi-get-parameters-for-export-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-export-output-schema.json\",\n  \"title\": \"GetParametersForExportOutput\",\n  \"description\": \"GetParametersForExportOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExportToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportTokenId\"\n        },\n        {\n          \"description\": \"The export token to initiate key export from Amazon Web Services Payment Cryptography. The export token expires after 7 days. You can use the same export token to export multiple keys from the same service account.\"\n        }\n      ]\n    },\n    \"ParametersValidUntilTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n \
  \       {\n          \"description\": \"The validity period of the export token.\"\n        }\n      ]\n    },\n    \"SigningKeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAlgorithm\"\n        },\n        {\n          \"description\": \"The algorithm of the signing key certificate for use in TR-34 key block generation. <code>RSA_2048</code> is the only signing key algorithm allowed.\"\n        }\n      ]\n    },\n    \"SigningKeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The signing key certificate of the public key for signature within the TR-34 key block cryptogram. The certificate expires after 7 days.\"\n        }\n      ]\n    },\n    \"SigningKeyCertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The\
  \ certificate chain that signed the signing key certificate. This is the root certificate authority (CA) within your service account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ExportToken\",\n    \"ParametersValidUntilTimestamp\",\n    \"SigningKeyAlgorithm\",\n    \"SigningKeyCertificate\",\n    \"SigningKeyCertificateChain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-parameters-for-export-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetParametersForExportOutput
---
