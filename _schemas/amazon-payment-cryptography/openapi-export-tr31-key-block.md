---
description: Parameter information for key material export using TR-31 standard.
layout: schema
name: ExportTr31KeyBlock
properties_list:
- description: ''
  name: WrappingKeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-export-tr31-key-block-schema.json
slug: openapi-export-tr31-key-block
source_filename: openapi-export-tr31-key-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-tr31-key-block-schema.json\",\n  \"title\": \"ExportTr31KeyBlock\",\n  \"description\": \"Parameter information for key material export using TR-31 standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WrappingKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the the wrapping key. This key encrypts or wraps the key under export for TR-31 key block generation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"WrappingKeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-tr31-key-block-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ExportTr31KeyBlock
---
