---
description: ListKeysInput schema from Amazon Payment Cryptography
layout: schema
name: ListKeysInput
properties_list:
- description: ''
  name: KeyState
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-list-keys-input-schema.json
slug: openapi-list-keys-input
source_filename: openapi-list-keys-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-keys-input-schema.json\",\n  \"title\": \"ListKeysInput\",\n  \"description\": \"ListKeysInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyState\"\n        },\n        {\n          \"description\": \"The key state of the keys you want to list.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"Use this parameter to specify the maximum number of items to return. When this value is present, Amazon Web Services Payment Cryptography does not return more than the specified number of items, but it might\
  \ return fewer.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Use this parameter in a subsequent request after you receive a response with truncated results. Set it to the value of <code>NextToken</code> from the truncated response you just received.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-keys-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ListKeysInput
---
