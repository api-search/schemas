---
description: Parameter information for key material export using TR-34 standard.
layout: schema
name: ExportTr34KeyBlock
properties_list:
- description: ''
  name: CertificateAuthorityPublicKeyIdentifier
  type: object
- description: ''
  name: ExportToken
  type: object
- description: ''
  name: KeyBlockFormat
  type: object
- description: ''
  name: RandomNonce
  type: object
- description: ''
  name: WrappingKeyCertificate
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-export-tr34-key-block-schema.json
slug: openapi-export-tr34-key-block
source_filename: openapi-export-tr34-key-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-tr34-key-block-schema.json\",\n  \"title\": \"ExportTr34KeyBlock\",\n  \"description\": \"Parameter information for key material export using TR-34 standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityPublicKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the certificate chain that signs the wrapping key certificate during TR-34 key export.\"\n        }\n      ]\n    },\n    \"ExportToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportTokenId\"\n        },\n        {\n          \"description\": \"The export token to initiate key export from Amazon Web Services\
  \ Payment Cryptography. It also contains the signing key certificate that will sign the wrapped key during TR-34 key block generation. Call <a>GetParametersForExport</a> to receive an export token. It expires after 7 days. You can use the same export token to export multiple keys from the same service account.\"\n        }\n      ]\n    },\n    \"KeyBlockFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tr34KeyBlockFormat\"\n        },\n        {\n          \"description\": \"The format of key block that Amazon Web Services Payment Cryptography will use during key export.\"\n        }\n      ]\n    },\n    \"RandomNonce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HexLength16\"\n        },\n        {\n          \"description\": \"A random number value that is unique to the TR-34 key block generated using 2 pass. The operation will fail, if a random nonce value is not provided for a TR-34 key block generated using 2\
  \ pass.\"\n        }\n      ]\n    },\n    \"WrappingKeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the wrapping key certificate. Amazon Web Services Payment Cryptography uses this certificate to wrap the key under export.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityPublicKeyIdentifier\",\n    \"ExportToken\",\n    \"KeyBlockFormat\",\n    \"WrappingKeyCertificate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-tr34-key-block-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ExportTr34KeyBlock
---
