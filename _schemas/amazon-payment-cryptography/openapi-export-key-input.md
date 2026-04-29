---
description: ExportKeyInput schema from Amazon Payment Cryptography
layout: schema
name: ExportKeyInput
properties_list:
- description: ''
  name: ExportKeyIdentifier
  type: object
- description: ''
  name: KeyMaterial
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-export-key-input-schema.json
slug: openapi-export-key-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-input-schema.json\",\n  \"title\": \"ExportKeyInput\",\n  \"description\": \"ExportKeyInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExportKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key under export from Amazon Web Services Payment Cryptography.\"\n        }\n      ]\n    },\n    \"KeyMaterial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportKeyMaterial\"\n        },\n        {\n          \"description\": \"The key block format type, for example, TR-34 or TR-31, to use during key material export.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"ExportKeyIdentifier\",\n    \"KeyMaterial\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ExportKeyInput
---
