---
description: Contains information about an alias.
layout: schema
name: Alias
properties_list:
- description: ''
  name: AliasName
  type: object
- description: ''
  name: KeyArn
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-alias-schema.json
slug: openapi-alias
source_filename: openapi-alias-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-alias-schema.json\",\n  \"title\": \"Alias\",\n  \"description\": \"Contains information about an alias.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasName\"\n        },\n        {\n          \"description\": \"<p>A friendly name that you can use to refer to a key. The value must begin with <code>alias/</code>.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important>\"\n        }\n      ]\n    },\n    \"KeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code>\
  \ of the key associated with the alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-alias-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: Alias
---
