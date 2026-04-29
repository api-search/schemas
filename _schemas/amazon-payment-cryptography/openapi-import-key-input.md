---
description: ImportKeyInput schema from Amazon Payment Cryptography
layout: schema
name: ImportKeyInput
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: KeyCheckValueAlgorithm
  type: object
- description: ''
  name: KeyMaterial
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-import-key-input-schema.json
slug: openapi-import-key-input
source_filename: openapi-import-key-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-key-input-schema.json\",\n  \"title\": \"ImportKeyInput\",\n  \"description\": \"ImportKeyInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether import key is enabled.\"\n        }\n      ]\n    },\n    \"KeyCheckValueAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyCheckValueAlgorithm\"\n        },\n        {\n          \"description\": \"<p>The algorithm that Amazon Web Services Payment Cryptography uses to calculate the key check value (KCV) for DES and AES keys.</p> <p>For DES key, the KCV is computed by encrypting 8\
  \ bytes, each with value '00', with the key to be checked and retaining the 3 highest order bytes of the encrypted result. For AES key, the KCV is computed by encrypting 8 bytes, each with value '01', with the key to be checked and retaining the 3 highest order bytes of the encrypted result.</p>\"\n        }\n      ]\n    },\n    \"KeyMaterial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportKeyMaterial\"\n        },\n        {\n          \"description\": \"The key or public key certificate type to use during key material import, for example TR-34 or RootCertificatePublicKey.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>The tags to attach to the key. Each tag consists of a tag key and a tag value. Both the tag key and the tag value are required, but the tag value can be an empty (null) string. You can't have more\
  \ than one tag on an Amazon Web Services Payment Cryptography key with the same tag key. </p> <p>You can't have more than one tag on an Amazon Web Services Payment Cryptography key with the same tag key. If you specify an existing tag key with a different tag value, Amazon Web Services Payment Cryptography replaces the current tag value with the specified one.</p> <p>To use this parameter, you must have <code>TagResource</code> permission.</p> <important> <p>Don't include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <note> <p>Tagging or untagging an Amazon Web Services Payment Cryptography key can allow or deny permission to the key.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyMaterial\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-key-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ImportKeyInput
---
