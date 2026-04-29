---
description: KeyArnOrKeyAliasType schema from Amazon Payment Cryptography
layout: schema
name: KeyArnOrKeyAliasType
properties_list: []
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-key-arn-or-key-alias-type-schema.json
slug: openapi-key-arn-or-key-alias-type
source_filename: openapi-key-arn-or-key-alias-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-arn-or-key-alias-type-schema.json\",\n  \"title\": \"KeyArnOrKeyAliasType\",\n  \"description\": \"KeyArnOrKeyAliasType schema from Amazon Payment Cryptography\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws:payment-cryptography:[a-z]{2}-[a-z]{1,16}-[0-9]+:[0-9]{12}:(key/[0-9a-zA-Z]{16,64}|alias/[a-zA-Z0-9/_-]+)$|^alias/[a-zA-Z0-9/_-]+$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-arn-or-key-alias-type-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: KeyArnOrKeyAliasType
---
