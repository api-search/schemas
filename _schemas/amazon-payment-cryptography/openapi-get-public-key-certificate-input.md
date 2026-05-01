---
description: GetPublicKeyCertificateInput schema from Amazon Payment Cryptography
layout: schema
name: GetPublicKeyCertificateInput
properties_list:
- description: ''
  name: KeyIdentifier
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-public-key-certificate-input-schema.json
slug: openapi-get-public-key-certificate-input
source_filename: openapi-get-public-key-certificate-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-public-key-certificate-input-schema.json\",\n  \"title\": \"GetPublicKeyCertificateInput\",\n  \"description\": \"GetPublicKeyCertificateInput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the asymmetric key pair.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-public-key-certificate-input-schema.json
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetPublicKeyCertificateInput
---
