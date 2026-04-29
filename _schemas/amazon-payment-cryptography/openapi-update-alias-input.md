---
description: UpdateAliasInput schema from Amazon Payment Cryptography
layout: schema
name: UpdateAliasInput
properties_list:
- description: ''
  name: AliasName
  type: object
- description: ''
  name: KeyArn
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-update-alias-input-schema.json
slug: openapi-update-alias-input
source_filename: openapi-update-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-update-alias-input-schema.json\",\n  \"title\": \"UpdateAliasInput\",\n  \"description\": \"UpdateAliasInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasName\"\n        },\n        {\n          \"description\": \"The alias whose associated key is changing.\"\n        }\n      ]\n    },\n    \"KeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> for the key that you are updating or removing from the alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-update-alias-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: UpdateAliasInput
---
