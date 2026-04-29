---
description: DeleteKeyInput schema from Amazon Payment Cryptography
layout: schema
name: DeleteKeyInput
properties_list:
- description: ''
  name: DeleteKeyInDays
  type: object
- description: ''
  name: KeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-delete-key-input-schema.json
slug: openapi-delete-key-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-delete-key-input-schema.json\",\n  \"title\": \"DeleteKeyInput\",\n  \"description\": \"DeleteKeyInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeleteKeyInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeleteKeyInputDeleteKeyInDaysInteger\"\n        },\n        {\n          \"description\": \"The waiting period for key deletion. The default value is seven days.\"\n        }\n      ]\n    },\n    \"KeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key that is scheduled for deletion.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  KeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-delete-key-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: DeleteKeyInput
---
