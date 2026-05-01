---
description: The list of cryptographic operations that you can perform using the key. The modes of use are deﬁned in section A.5.3 of the TR-31 spec.
layout: schema
name: KeyModesOfUse
properties_list:
- description: ''
  name: Decrypt
  type: object
- description: ''
  name: DeriveKey
  type: object
- description: ''
  name: Encrypt
  type: object
- description: ''
  name: Generate
  type: object
- description: ''
  name: NoRestrictions
  type: object
- description: ''
  name: Sign
  type: object
- description: ''
  name: Unwrap
  type: object
- description: ''
  name: Verify
  type: object
- description: ''
  name: Wrap
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-key-modes-of-use-schema.json
slug: openapi-key-modes-of-use
source_filename: openapi-key-modes-of-use-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-modes-of-use-schema.json\",\n  \"title\": \"KeyModesOfUse\",\n  \"description\": \"The list of cryptographic operations that you can perform using the key. The modes of use are de\\ufb01ned in section A.5.3 of the TR-31 spec.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Decrypt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to decrypt data.\"\n        }\n      ]\n    },\n    \"DeriveKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment\
  \ Cryptography key can be used to derive new keys.\"\n        }\n      ]\n    },\n    \"Encrypt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to encrypt data.\"\n        }\n      ]\n    },\n    \"Generate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to generate and verify other card and PIN verification keys.\"\n        }\n      ]\n    },\n    \"NoRestrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key has no special restrictions other than\
  \ the restrictions implied by <code>KeyUsage</code>.\"\n        }\n      ]\n    },\n    \"Sign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used for signing.\"\n        }\n      ]\n    },\n    \"Unwrap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to unwrap other keys.\"\n        }\n      ]\n    },\n    \"Verify\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to verify signatures.\"\n        }\n      ]\n    },\n    \"Wrap\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimitiveBoolean\"\n        },\n        {\n          \"description\": \"Speci\\ufb01es whether an Amazon Web Services Payment Cryptography key can be used to wrap other keys.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-modes-of-use-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: KeyModesOfUse
---
