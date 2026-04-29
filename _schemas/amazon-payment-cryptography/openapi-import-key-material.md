---
description: Parameter information for key material import.
layout: schema
name: ImportKeyMaterial
properties_list:
- description: ''
  name: RootCertificatePublicKey
  type: object
- description: ''
  name: Tr31KeyBlock
  type: object
- description: ''
  name: Tr34KeyBlock
  type: object
- description: ''
  name: TrustedCertificatePublicKey
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-import-key-material-schema.json
slug: openapi-import-key-material
source_filename: openapi-import-key-material-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-key-material-schema.json\",\n  \"title\": \"ImportKeyMaterial\",\n  \"description\": \"Parameter information for key material import.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RootCertificatePublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RootCertificatePublicKey\"\n        },\n        {\n          \"description\": \"Parameter information for root public key certificate import.\"\n        }\n      ]\n    },\n    \"Tr31KeyBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportTr31KeyBlock\"\n        },\n        {\n          \"description\": \"Parameter information for key material import using TR-31 standard.\"\n        }\n      ]\n    },\n    \"Tr34KeyBlock\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ImportTr34KeyBlock\"\n        },\n        {\n          \"description\": \"Parameter information for key material import using TR-34 standard.\"\n        }\n      ]\n    },\n    \"TrustedCertificatePublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustedCertificatePublicKey\"\n        },\n        {\n          \"description\": \"Parameter information for trusted public key certificate import.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-import-key-material-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: ImportKeyMaterial
---
