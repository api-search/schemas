---
description: Parameter information for key material import using TR-34 standard.
layout: schema
name: ImportTr34KeyBlock
properties_list:
- description: ''
  name: CertificateAuthorityPublicKeyIdentifier
  type: object
- description: ''
  name: ImportToken
  type: object
- description: ''
  name: KeyBlockFormat
  type: object
- description: ''
  name: RandomNonce
  type: object
- description: ''
  name: SigningKeyCertificate
  type: object
- description: ''
  name: WrappedKeyBlock
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-import-tr34-key-block-schema.json
slug: openapi-import-tr34-key-block
source_filename: openapi-import-tr34-key-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-tr34-key-block-schema.json\",\n  \"title\": \"ImportTr34KeyBlock\",\n  \"description\": \"Parameter information for key material import using TR-34 standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityPublicKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the certificate chain that signs the signing key certificate during TR-34 key import.\"\n        }\n      ]\n    },\n    \"ImportToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportTokenId\"\n        },\n        {\n          \"description\": \"The import token that initiates key import into Amazon Web Services\
  \ Payment Cryptography. It expires after 7 days. You can use the same import token to import multiple keys to the same service account.\"\n        }\n      ]\n    },\n    \"KeyBlockFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tr34KeyBlockFormat\"\n        },\n        {\n          \"description\": \"The key block format to use during key import. The only value allowed is <code>X9_TR34_2012</code>.\"\n        }\n      ]\n    },\n    \"RandomNonce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HexLength16\"\n        },\n        {\n          \"description\": \"A random number value that is unique to the TR-34 key block generated using 2 pass. The operation will fail, if a random nonce value is not provided for a TR-34 key block generated using 2 pass.\"\n        }\n      ]\n    },\n    \"SigningKeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n\
  \        {\n          \"description\": \"The public key component in PEM certificate format of the private key that signs the KDH TR-34 wrapped key block.\"\n        }\n      ]\n    },\n    \"WrappedKeyBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tr34WrappedKeyBlock\"\n        },\n        {\n          \"description\": \"The TR-34 wrapped key block to import.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityPublicKeyIdentifier\",\n    \"ImportToken\",\n    \"KeyBlockFormat\",\n    \"SigningKeyCertificate\",\n    \"WrappedKeyBlock\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-tr34-key-block-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ImportTr34KeyBlock
---
