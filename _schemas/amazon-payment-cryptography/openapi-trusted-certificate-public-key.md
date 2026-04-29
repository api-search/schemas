---
description: Parameter information for trusted public key certificate import.
layout: schema
name: TrustedCertificatePublicKey
properties_list:
- description: ''
  name: CertificateAuthorityPublicKeyIdentifier
  type: object
- description: ''
  name: KeyAttributes
  type: object
- description: ''
  name: PublicKeyCertificate
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-trusted-certificate-public-key-schema.json
slug: openapi-trusted-certificate-public-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-trusted-certificate-public-key-schema.json\",\n  \"title\": \"TrustedCertificatePublicKey\",\n  \"description\": \"Parameter information for trusted public key certificate import.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityPublicKeyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArnOrKeyAliasType\"\n        },\n        {\n          \"description\": \"The <code>KeyARN</code> of the root public key certificate or certificate chain that signs the trusted public key certificate import.\"\n        }\n      ]\n    },\n    \"KeyAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAttributes\"\n        },\n        {\n          \"description\": \"The role of the key, the algorithm\
  \ it supports, and the cryptographic operations allowed with the key. This data is immutable after a trusted public key is imported.\"\n        }\n      ]\n    },\n    \"PublicKeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"Parameter information for trusted public key certificate import.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityPublicKeyIdentifier\",\n    \"KeyAttributes\",\n    \"PublicKeyCertificate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-trusted-certificate-public-key-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: TrustedCertificatePublicKey
---
