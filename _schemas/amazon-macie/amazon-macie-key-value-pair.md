---
description: Provides information about the tags that are associated with an S3 bucket or object. Each tag consists of a required tag key and an associated tag value.
layout: schema
name: KeyValuePair
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-key-value-pair-schema.json
slug: amazon-macie-key-value-pair
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-key-value-pair-schema.json\",\n  \"title\": \"KeyValuePair\",\n  \"description\": \"Provides information about the tags that are associated with an S3 bucket or object. Each tag consists of a required tag key and an associated tag value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"One part of a key-value pair that comprises a tag. A tag key is a general label that acts as a category for more specific tag values.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"One part of a key-value pair that comprises\
  \ a tag. A tag value acts as a descriptor for a tag key. A tag value can be an empty string.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-key-value-pair-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: KeyValuePair
---
