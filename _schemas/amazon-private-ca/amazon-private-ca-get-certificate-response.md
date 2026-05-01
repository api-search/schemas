---
description: GetCertificateResponse schema from Amazon Private CA API
layout: schema
name: GetCertificateResponse
properties_list:
- description: ''
  name: Certificate
  type: object
- description: ''
  name: CertificateChain
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-get-certificate-response-schema.json
slug: amazon-private-ca-get-certificate-response
source_filename: amazon-private-ca-get-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-response-schema.json\",\n  \"title\": \"GetCertificateResponse\",\n  \"description\": \"GetCertificateResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBody\"\n        },\n        {\n          \"description\": \"The base64 PEM-encoded certificate specified by the <code>CertificateArn</code> parameter.\"\n        }\n      ]\n    },\n    \"CertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateChain\"\n        },\n        {\n          \"description\": \"The base64 PEM-encoded certificate chain that chains up to the root CA certificate that you used to sign your private\
  \ CA certificate. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-response-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GetCertificateResponse
---
