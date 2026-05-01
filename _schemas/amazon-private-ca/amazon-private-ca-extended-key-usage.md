---
description: Specifies additional purposes for which the certified public key may be used other than basic purposes indicated in the <code>KeyUsage</code> extension.
layout: schema
name: ExtendedKeyUsage
properties_list:
- description: ''
  name: ExtendedKeyUsageType
  type: object
- description: ''
  name: ExtendedKeyUsageObjectIdentifier
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-extended-key-usage-schema.json
slug: amazon-private-ca-extended-key-usage
source_filename: amazon-private-ca-extended-key-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-extended-key-usage-schema.json\",\n  \"title\": \"ExtendedKeyUsage\",\n  \"description\": \"Specifies additional purposes for which the certified public key may be used other than basic purposes indicated in the <code>KeyUsage</code> extension.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExtendedKeyUsageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExtendedKeyUsageType\"\n        },\n        {\n          \"description\": \"Specifies a standard <code>ExtendedKeyUsage</code> as defined as in <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12\\\">RFC 5280</a>.\"\n        }\n      ]\n    },\n    \"ExtendedKeyUsageObjectIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomObjectIdentifier\"\
  \n        },\n        {\n          \"description\": \"Specifies a custom <code>ExtendedKeyUsage</code> with an object identifier (OID).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-extended-key-usage-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ExtendedKeyUsage
---
