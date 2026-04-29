---
description: The role of the key, the algorithm it supports, and the cryptographic operations allowed with the key. This data is immutable after the key is created.
layout: schema
name: KeyAttributes
properties_list:
- description: ''
  name: KeyAlgorithm
  type: object
- description: ''
  name: KeyClass
  type: object
- description: ''
  name: KeyModesOfUse
  type: object
- description: ''
  name: KeyUsage
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-key-attributes-schema.json
slug: openapi-key-attributes
source_filename: openapi-key-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-attributes-schema.json\",\n  \"title\": \"KeyAttributes\",\n  \"description\": \"The role of the key, the algorithm it supports, and the cryptographic operations allowed with the key. This data is immutable after the key is created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAlgorithm\"\n        },\n        {\n          \"description\": \"<p>The key algorithm to be use during creation of an Amazon Web Services Payment Cryptography key.</p> <p>For symmetric keys, Amazon Web Services Payment Cryptography supports <code>AES</code> and <code>TDES</code> algorithms. For asymmetric keys, Amazon Web Services Payment Cryptography supports <code>RSA</code> and <code>ECC_NIST</code>\
  \ algorithms.</p>\"\n        }\n      ]\n    },\n    \"KeyClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyClass\"\n        },\n        {\n          \"description\": \"The type of Amazon Web Services Payment Cryptography key to create, which determines the classi\\ufb01cation of the cryptographic method and whether Amazon Web Services Payment Cryptography key contains a symmetric key or an asymmetric key pair.\"\n        }\n      ]\n    },\n    \"KeyModesOfUse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyModesOfUse\"\n        },\n        {\n          \"description\": \"The list of cryptographic operations that you can perform using the key.\"\n        }\n      ]\n    },\n    \"KeyUsage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyUsage\"\n        },\n        {\n          \"description\": \"The cryptographic usage of an Amazon Web Services Payment Cryptography key as de\\\
  ufb01ned in section A.5.2 of the TR-31 spec.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyAlgorithm\",\n    \"KeyClass\",\n    \"KeyModesOfUse\",\n    \"KeyUsage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-attributes-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: KeyAttributes
---
