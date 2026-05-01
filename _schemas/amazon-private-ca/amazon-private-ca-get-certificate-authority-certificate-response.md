---
description: GetCertificateAuthorityCertificateResponse schema from Amazon Private CA API
layout: schema
name: GetCertificateAuthorityCertificateResponse
properties_list:
- description: ''
  name: Certificate
  type: object
- description: ''
  name: CertificateChain
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-get-certificate-authority-certificate-response-schema.json
slug: amazon-private-ca-get-certificate-authority-certificate-response
source_filename: amazon-private-ca-get-certificate-authority-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-authority-certificate-response-schema.json\",\n  \"title\": \"GetCertificateAuthorityCertificateResponse\",\n  \"description\": \"GetCertificateAuthorityCertificateResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBody\"\n        },\n        {\n          \"description\": \"Base64-encoded certificate authority (CA) certificate.\"\n        }\n      ]\n    },\n    \"CertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateChain\"\n        },\n        {\n          \"description\": \"Base64-encoded certificate chain that includes any intermediate certificates and chains up\
  \ to root certificate that you used to sign your private CA certificate. The chain does not include your private CA certificate. If this is a root CA, the value will be null.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-authority-certificate-response-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GetCertificateAuthorityCertificateResponse
---
