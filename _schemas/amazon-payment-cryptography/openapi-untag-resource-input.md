---
description: UntagResourceInput schema from Amazon Payment Cryptography
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-untag-resource-input-schema.json
slug: openapi-untag-resource-input
source_filename: openapi-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key whose tags are being removed.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeys\"\n        },\n        {\n          \"description\": \"<p>One or more tag keys. Don't include the tag values.</p> <p>If the Amazon Web Services Payment Cryptography key doesn't have the specified tag key, Amazon Web Services\
  \ Payment Cryptography doesn't throw an exception or return a response. To confirm that the operation succeeded, use the <a>ListTagsForResource</a> operation.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-untag-resource-input-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: UntagResourceInput
---
