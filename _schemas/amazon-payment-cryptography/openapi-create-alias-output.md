---
description: CreateAliasOutput schema from Amazon Payment Cryptography
layout: schema
name: CreateAliasOutput
properties_list:
- description: ''
  name: Alias
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-create-alias-output-schema.json
slug: openapi-create-alias-output
source_filename: openapi-create-alias-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-alias-output-schema.json\",\n  \"title\": \"CreateAliasOutput\",\n  \"description\": \"CreateAliasOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alias\"\n        },\n        {\n          \"description\": \"The alias for the key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Alias\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-alias-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: CreateAliasOutput
---
