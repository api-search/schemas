---
description: DeleteCertificateAuthorityRequest schema from Amazon Private CA API
layout: schema
name: DeleteCertificateAuthorityRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: PermanentDeletionTimeInDays
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-delete-certificate-authority-request-schema.json
slug: amazon-private-ca-delete-certificate-authority-request
source_filename: amazon-private-ca-delete-certificate-authority-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-certificate-authority-request-schema.json\",\n  \"title\": \"DeleteCertificateAuthorityRequest\",\n  \"description\": \"DeleteCertificateAuthorityRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that was returned when you called <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a>. This must have the following form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code>.\
  \ </p>\"\n        }\n      ]\n    },\n    \"PermanentDeletionTimeInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermanentDeletionTimeInDays\"\n        },\n        {\n          \"description\": \"The number of days to make a CA restorable after it has been deleted. This can be anywhere from 7 to 30 days, with 30 being the default.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-certificate-authority-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DeleteCertificateAuthorityRequest
---
