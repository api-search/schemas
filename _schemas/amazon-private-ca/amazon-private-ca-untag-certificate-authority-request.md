---
description: UntagCertificateAuthorityRequest schema from Amazon Private CA API
layout: schema
name: UntagCertificateAuthorityRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-untag-certificate-authority-request-schema.json
slug: amazon-private-ca-untag-certificate-authority-request
source_filename: amazon-private-ca-untag-certificate-authority-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-untag-certificate-authority-request-schema.json\",\n  \"title\": \"UntagCertificateAuthorityRequest\",\n  \"description\": \"UntagCertificateAuthorityRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that was returned when you called <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a>. This must be of the form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code> </p>\"\n   \
  \     }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"List of tags to be removed from the CA.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-untag-certificate-authority-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: UntagCertificateAuthorityRequest
---
