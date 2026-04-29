---
description: ExportKeyOutput schema from Amazon Payment Cryptography
layout: schema
name: ExportKeyOutput
properties_list:
- description: ''
  name: WrappedKey
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-export-key-output-schema.json
slug: openapi-export-key-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-output-schema.json\",\n  \"title\": \"ExportKeyOutput\",\n  \"description\": \"ExportKeyOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WrappedKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedKey\"\n        },\n        {\n          \"description\": \"The key material under export as a TR-34 or TR-31 wrapped key block.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ExportKeyOutput
---
