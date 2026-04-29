---
description: Parameter information for key material export from Amazon Web Services Payment Cryptography.
layout: schema
name: ExportKeyMaterial
properties_list:
- description: ''
  name: Tr31KeyBlock
  type: object
- description: ''
  name: Tr34KeyBlock
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-export-key-material-schema.json
slug: openapi-export-key-material
source_filename: openapi-export-key-material-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-material-schema.json\",\n  \"title\": \"ExportKeyMaterial\",\n  \"description\": \"Parameter information for key material export from Amazon Web Services Payment Cryptography.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tr31KeyBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportTr31KeyBlock\"\n        },\n        {\n          \"description\": \"Parameter information for key material export using TR-31 standard.\"\n        }\n      ]\n    },\n    \"Tr34KeyBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportTr34KeyBlock\"\n        },\n        {\n          \"description\": \"Parameter information for key material export using TR-34 standard.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-export-key-material-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ExportKeyMaterial
---
