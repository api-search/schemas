---
description: CreateAliasInput schema from Amazon Payment Cryptography
layout: schema
name: CreateAliasInput
properties_list:
- description: ''
  name: AliasName
  type: object
- description: ''
  name: KeyArn
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-create-alias-input-schema.json
slug: openapi-create-alias-input
source_filename: openapi-create-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-alias-input-schema.json\",\n  \"title\": \"CreateAliasInput\",\n  \"description\": \"CreateAliasInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasName\"\n        },\n        {\n          \"description\": \"<p>A friendly name that you can use to refer a key. An alias must begin with <code>alias/</code> followed by a name, for example <code>alias/ExampleAlias</code>. It can contain only alphanumeric characters, forward slashes (/), underscores (_), and dashes (-).</p> <important> <p>Don't include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important>\"\
  \n        }\n      ]\n    },\n    \"KeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the key to associate with the alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-create-alias-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: CreateAliasInput
---
