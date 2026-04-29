---
description: GetAliasOutput schema from Amazon Payment Cryptography
layout: schema
name: GetAliasOutput
properties_list:
- description: ''
  name: Alias
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-alias-output-schema.json
slug: openapi-get-alias-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-alias-output-schema.json\",\n  \"title\": \"GetAliasOutput\",\n  \"description\": \"GetAliasOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alias\"\n        },\n        {\n          \"description\": \"The alias of the Amazon Web Services Payment Cryptography key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Alias\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-alias-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetAliasOutput
---
