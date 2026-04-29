---
description: Parameter information for key material import using TR-31 standard.
layout: schema
name: ImportTr31KeyBlock
properties_list:
- description: ''
  name: WrappedKeyBlock
  type: object
- description: ''
  name: WrappingKeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-import-tr31-key-block-schema.json
slug: openapi-import-tr31-key-block
source_filename: openapi-import-tr31-key-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-tr31-key-block-schema.json\",\n  \"title\": \"ImportTr31KeyBlock\",\n  \"description\": \"Parameter information for key material import using TR-31 standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WrappedKeyBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tr31WrappedKeyBlock\"\n        },\n        {\n          \"description\": \"The TR-34 wrapped key block to import.\"\n        }\n      ]\n    },\n    \"WrappingKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key that will decrypt or unwrap a TR-31 key block during import.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"WrappedKeyBlock\",\n    \"WrappingKeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-tr31-key-block-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ImportTr31KeyBlock
---
