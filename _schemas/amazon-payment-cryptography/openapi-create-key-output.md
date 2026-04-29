---
description: CreateKeyOutput schema from Amazon Payment Cryptography
layout: schema
name: CreateKeyOutput
properties_list:
- description: ''
  name: Key
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-create-key-output-schema.json
slug: openapi-create-key-output
source_filename: openapi-create-key-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-key-output-schema.json\",\n  \"title\": \"CreateKeyOutput\",\n  \"description\": \"CreateKeyOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The key material that contains all the key attributes.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-key-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: CreateKeyOutput
---
