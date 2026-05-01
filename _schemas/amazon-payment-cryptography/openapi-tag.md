---
description: A structure that contains information about a tag.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-tag-schema.json
slug: openapi-tag
source_filename: openapi-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A structure that contains information about a tag.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"The key of the tag.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"The value of the tag.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-tag-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: Tag
---
