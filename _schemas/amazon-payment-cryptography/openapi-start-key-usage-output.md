---
description: StartKeyUsageOutput schema from Amazon Payment Cryptography
layout: schema
name: StartKeyUsageOutput
properties_list:
- description: ''
  name: Key
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-start-key-usage-output-schema.json
slug: openapi-start-key-usage-output
source_filename: openapi-start-key-usage-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-start-key-usage-output-schema.json\",\n  \"title\": \"StartKeyUsageOutput\",\n  \"description\": \"StartKeyUsageOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the Amazon Web Services Payment Cryptography key activated for use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-start-key-usage-output-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: StartKeyUsageOutput
---
