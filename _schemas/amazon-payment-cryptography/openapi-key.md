---
description: Metadata about an Amazon Web Services Payment Cryptography key.
layout: schema
name: Key
properties_list:
- description: ''
  name: CreateTimestamp
  type: object
- description: ''
  name: DeletePendingTimestamp
  type: object
- description: ''
  name: DeleteTimestamp
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: Exportable
  type: object
- description: ''
  name: KeyArn
  type: object
- description: ''
  name: KeyAttributes
  type: object
- description: ''
  name: KeyCheckValue
  type: object
- description: ''
  name: KeyCheckValueAlgorithm
  type: object
- description: ''
  name: KeyOrigin
  type: object
- description: ''
  name: KeyState
  type: object
- description: ''
  name: UsageStartTimestamp
  type: object
- description: ''
  name: UsageStopTimestamp
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-key-schema.json
slug: openapi-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-schema.json\",\n  \"title\": \"Key\",\n  \"description\": \"Metadata about an Amazon Web Services Payment Cryptography key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the key was created.\"\n        }\n      ]\n    },\n    \"DeletePendingTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time after which Amazon Web Services Payment Cryptography will delete the key. This value is present only when <code>KeyState</code> is <code>DELETE_PENDING</code> and the key is scheduled\
  \ for deletion.\"\n        }\n      ]\n    },\n    \"DeleteTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time after which Amazon Web Services Payment Cryptography will delete the key. This value is present only when when the <code>KeyState</code> is <code>DELETE_COMPLETE</code> and the Amazon Web Services Payment Cryptography key is deleted.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the key is enabled. \"\n        }\n      ]\n    },\n    \"Exportable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the key is exportable. This data is immutable after the key is created.\"\n        }\n      ]\n  \
  \  },\n    \"KeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the key.\"\n        }\n      ]\n    },\n    \"KeyAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAttributes\"\n        },\n        {\n          \"description\": \"The role of the key, the algorithm it supports, and the cryptographic operations allowed with the key. This data is immutable after the key is created.\"\n        }\n      ]\n    },\n    \"KeyCheckValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyCheckValue\"\n        },\n        {\n          \"description\": \"The key check value (KCV) is used to check if all parties holding a given key have the same key or to detect that a key has changed. Amazon Web Services Payment Cryptography calculates the KCV by using standard algorithms, typically by encrypting\
  \ 8 or 16 bytes or \\\"00\\\" or \\\"01\\\" and then truncating the result to the first 3 bytes, or 6 hex digits, of the resulting cryptogram.\"\n        }\n      ]\n    },\n    \"KeyCheckValueAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyCheckValueAlgorithm\"\n        },\n        {\n          \"description\": \"The algorithm used for calculating key check value (KCV) for DES and AES keys. For a DES key, Amazon Web Services Payment Cryptography computes the KCV by encrypting 8 bytes, each with value '00', with the key to be checked and retaining the 3 highest order bytes of the encrypted result. For an AES key, Amazon Web Services Payment Cryptography computes the KCV by encrypting 8 bytes, each with value '01', with the key to be checked and retaining the 3 highest order bytes of the encrypted result.\"\n        }\n      ]\n    },\n    \"KeyOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyOrigin\"\n\
  \        },\n        {\n          \"description\": \"The source of the key material. For keys created within Amazon Web Services Payment Cryptography, the value is <code>AWS_PAYMENT_CRYPTOGRAPHY</code>. For keys imported into Amazon Web Services Payment Cryptography, the value is <code>EXTERNAL</code>.\"\n        }\n      ]\n    },\n    \"KeyState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyState\"\n        },\n        {\n          \"description\": \"The state of key that is being created or deleted.\"\n        }\n      ]\n    },\n    \"UsageStartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time after which Amazon Web Services Payment Cryptography will start using the key material for cryptographic operations.\"\n        }\n      ]\n    },\n    \"UsageStopTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The date and time after which Amazon Web Services Payment Cryptography will stop using the key material for cryptographic operations.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreateTimestamp\",\n    \"Enabled\",\n    \"Exportable\",\n    \"KeyArn\",\n    \"KeyAttributes\",\n    \"KeyCheckValue\",\n    \"KeyCheckValueAlgorithm\",\n    \"KeyOrigin\",\n    \"KeyState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: Key
---
