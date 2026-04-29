---
description: GetCertificateAuthorityCsrResponse schema from Amazon Private CA API
layout: schema
name: GetCertificateAuthorityCsrResponse
properties_list:
- description: ''
  name: Csr
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-get-certificate-authority-csr-response-schema.json
slug: amazon-private-ca-get-certificate-authority-csr-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-authority-csr-response-schema.json\",\n  \"title\": \"GetCertificateAuthorityCsrResponse\",\n  \"description\": \"GetCertificateAuthorityCsrResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Csr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CsrBody\"\n        },\n        {\n          \"description\": \"The base64 PEM-encoded certificate signing request (CSR) for your private CA certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-certificate-authority-csr-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GetCertificateAuthorityCsrResponse
---
