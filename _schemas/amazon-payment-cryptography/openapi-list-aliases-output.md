---
description: ListAliasesOutput schema from Amazon Payment Cryptography
layout: schema
name: ListAliasesOutput
properties_list:
- description: ''
  name: Aliases
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-list-aliases-output-schema.json
slug: openapi-list-aliases-output
source_filename: openapi-list-aliases-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-aliases-output-schema.json\",\n  \"title\": \"ListAliasesOutput\",\n  \"description\": \"ListAliasesOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Aliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Aliases\"\n        },\n        {\n          \"description\": \"The list of aliases. Each alias describes the <code>KeyArn</code> contained within.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or an empty or null value if there are no more results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Aliases\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-aliases-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ListAliasesOutput
---
