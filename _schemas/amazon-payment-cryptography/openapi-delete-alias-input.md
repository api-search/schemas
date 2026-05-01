---
description: DeleteAliasInput schema from Amazon Payment Cryptography
layout: schema
name: DeleteAliasInput
properties_list:
- description: ''
  name: AliasName
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-delete-alias-input-schema.json
slug: openapi-delete-alias-input
source_filename: openapi-delete-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-delete-alias-input-schema.json\",\n  \"title\": \"DeleteAliasInput\",\n  \"description\": \"DeleteAliasInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasName\"\n        },\n        {\n          \"description\": \"A friendly name that you can use to refer Amazon Web Services Payment Cryptography key. This value must begin with <code>alias/</code> followed by a name, such as <code>alias/ExampleAlias</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-delete-alias-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: DeleteAliasInput
---
