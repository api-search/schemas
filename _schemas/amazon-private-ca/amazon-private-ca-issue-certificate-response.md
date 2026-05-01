---
description: IssueCertificateResponse schema from Amazon Private CA API
layout: schema
name: IssueCertificateResponse
properties_list:
- description: ''
  name: CertificateArn
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-issue-certificate-response-schema.json
slug: amazon-private-ca-issue-certificate-response
source_filename: amazon-private-ca-issue-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-issue-certificate-response-schema.json\",\n  \"title\": \"IssueCertificateResponse\",\n  \"description\": \"IssueCertificateResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the issued certificate and the certificate serial number. This is of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i>/certificate/<i>286535153982981100925020015808220737245</i> </code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-issue-certificate-response-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: IssueCertificateResponse
---
