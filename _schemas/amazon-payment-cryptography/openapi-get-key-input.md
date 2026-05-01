---
description: GetKeyInput schema from Amazon Payment Cryptography
layout: schema
name: GetKeyInput
properties_list:
- description: ''
  name: KeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-key-input-schema.json
slug: openapi-get-key-input
source_filename: openapi-get-key-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-key-input-schema.json\",\n  \"title\": \"GetKeyInput\",\n  \"description\": \"GetKeyInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the Amazon Web Services Payment Cryptography key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-key-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetKeyInput
---
