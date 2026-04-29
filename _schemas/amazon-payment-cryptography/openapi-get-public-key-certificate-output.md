---
description: GetPublicKeyCertificateOutput schema from Amazon Payment Cryptography
layout: schema
name: GetPublicKeyCertificateOutput
properties_list:
- description: ''
  name: KeyCertificate
  type: object
- description: ''
  name: KeyCertificateChain
  type: object
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-get-public-key-certificate-output-schema.json
slug: openapi-get-public-key-certificate-output
source_filename: openapi-get-public-key-certificate-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-public-key-certificate-output-schema.json\",\n  \"title\": \"GetPublicKeyCertificateOutput\",\n  \"description\": \"GetPublicKeyCertificateOutput schema from Amazon Payment Cryptography\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"The public key component of the asymmetric key pair in a certificate (PEM) format. It is signed by the root certificate authority (CA) within your service account. The certificate expires in 90 days.\"\n        }\n      ]\n    },\n    \"KeyCertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n \
  \         \"description\": \"The certificate chain that signed the public key certificate of the asymmetric key pair. This is the root certificate authority (CA) within your service account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyCertificate\",\n    \"KeyCertificateChain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-get-public-key-certificate-output-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: GetPublicKeyCertificateOutput
---
