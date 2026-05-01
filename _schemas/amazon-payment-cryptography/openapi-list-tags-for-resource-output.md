---
description: ListTagsForResourceOutput schema from Amazon Payment Cryptography
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-list-tags-for-resource-output-schema.json
slug: openapi-list-tags-for-resource-output
source_filename: openapi-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or an empty or null value if there are no more results.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The list of tags associated with a <code>ResourceArn</code>. Each tag will list the key-value pair contained within that tag.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-list-tags-for-resource-output-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ListTagsForResourceOutput
---
