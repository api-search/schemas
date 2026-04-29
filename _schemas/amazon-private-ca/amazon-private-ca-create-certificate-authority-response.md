---
description: CreateCertificateAuthorityResponse schema from Amazon Private CA API
layout: schema
name: CreateCertificateAuthorityResponse
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-create-certificate-authority-response-schema.json
slug: amazon-private-ca-create-certificate-authority-response
source_filename: amazon-private-ca-create-certificate-authority-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-response-schema.json\",\n  \"title\": \"CreateCertificateAuthorityResponse\",\n  \"description\": \"CreateCertificateAuthorityResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>If successful, the Amazon Resource Name (ARN) of the certificate authority (CA). This is of the form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code>. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CreateCertificateAuthorityResponse
---
