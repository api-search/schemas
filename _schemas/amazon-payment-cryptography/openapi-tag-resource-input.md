---
description: TagResourceInput schema from Amazon Payment Cryptography
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-tag-resource-input-schema.json
slug: openapi-tag-resource-input
source_filename: openapi-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key whose tags are being updated.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>One or more tags. Each tag consists of a tag key and a tag value. The tag value can be an empty (null) string. You can't have more than one tag on an Amazon Web Services Payment Cryptography\
  \ key with the same tag key. If you specify an existing tag key with a different tag value, Amazon Web Services Payment Cryptography replaces the current tag value with the new one.</p> <important> <p>Don't include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>To use this parameter, you must have <a>TagResource</a> permission in an IAM policy.</p> <important> <p>Don't include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-tag-resource-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: TagResourceInput
---
