---
description: ListKeysOutput schema from Amazon Payment Cryptography
layout: schema
name: ListKeysOutput
properties_list:
- description: ''
  name: Keys
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-list-keys-output-schema.json
slug: openapi-list-keys-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-keys-output-schema.json\",\n  \"title\": \"ListKeysOutput\",\n  \"description\": \"ListKeysOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Keys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeySummaryList\"\n        },\n        {\n          \"description\": \"The list of keys created within the caller's Amazon Web Services account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or an empty or null value if there are no more results.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Keys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-keys-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ListKeysOutput
---
