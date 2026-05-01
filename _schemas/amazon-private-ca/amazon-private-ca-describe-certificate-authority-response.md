---
description: DescribeCertificateAuthorityResponse schema from Amazon Private CA API
layout: schema
name: DescribeCertificateAuthorityResponse
properties_list:
- description: ''
  name: CertificateAuthority
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-describe-certificate-authority-response-schema.json
slug: amazon-private-ca-describe-certificate-authority-response
source_filename: amazon-private-ca-describe-certificate-authority-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-response-schema.json\",\n  \"title\": \"DescribeCertificateAuthorityResponse\",\n  \"description\": \"DescribeCertificateAuthorityResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthority\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CertificateAuthority.html\\\">CertificateAuthority</a> structure that contains information about your private CA.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-describe-certificate-authority-response-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DescribeCertificateAuthorityResponse
---
