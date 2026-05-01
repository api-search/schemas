---
description: Defines one or more purposes for which the key contained in the certificate can be used. Default value for each option is false.
layout: schema
name: KeyUsage
properties_list:
- description: ''
  name: DigitalSignature
  type: object
- description: ''
  name: NonRepudiation
  type: object
- description: ''
  name: KeyEncipherment
  type: object
- description: ''
  name: DataEncipherment
  type: object
- description: ''
  name: KeyAgreement
  type: object
- description: ''
  name: KeyCertSign
  type: object
- description: ''
  name: CRLSign
  type: object
- description: ''
  name: EncipherOnly
  type: object
- description: ''
  name: DecipherOnly
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-key-usage-schema.json
slug: amazon-private-ca-key-usage
source_filename: amazon-private-ca-key-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-key-usage-schema.json\",\n  \"title\": \"KeyUsage\",\n  \"description\": \"Defines one or more purposes for which the key contained in the certificate can be used. Default value for each option is false.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DigitalSignature\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Key can be used for digital signing.\"\n        }\n      ]\n    },\n    \"NonRepudiation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used for non-repudiation.\"\n        }\n      ]\n    },\n    \"KeyEncipherment\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used to encipher data.\"\n        }\n      ]\n    },\n    \"DataEncipherment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used to decipher data.\"\n        }\n      ]\n    },\n    \"KeyAgreement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used in a key-agreement protocol.\"\n        }\n      ]\n    },\n    \"KeyCertSign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used to sign certificates.\"\n        }\n      ]\n    },\n    \"CRLSign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \"Key can be used to sign CRLs.\"\n        }\n      ]\n    },\n    \"EncipherOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used only to encipher data.\"\n        }\n      ]\n    },\n    \"DecipherOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Key can be used only to decipher data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-key-usage-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: KeyUsage
---
