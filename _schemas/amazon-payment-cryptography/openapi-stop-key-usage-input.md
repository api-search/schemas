---
description: StopKeyUsageInput schema from Amazon Payment Cryptography
layout: schema
name: StopKeyUsageInput
properties_list:
- description: ''
  name: KeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-stop-key-usage-input-schema.json
slug: openapi-stop-key-usage-input
source_filename: openapi-stop-key-usage-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-stop-key-usage-input-schema.json\",\n  \"title\": \"StopKeyUsageInput\",\n  \"description\": \"StopKeyUsageInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyArn</code> of the key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-stop-key-usage-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: StopKeyUsageInput
---
