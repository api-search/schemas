---
description: DeletePermissionRequest schema from Amazon Private CA API
layout: schema
name: DeletePermissionRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: Principal
  type: object
- description: ''
  name: SourceAccount
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-delete-permission-request-schema.json
slug: amazon-private-ca-delete-permission-request
source_filename: amazon-private-ca-delete-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-permission-request-schema.json\",\n  \"title\": \"DeletePermissionRequest\",\n  \"description\": \"DeletePermissionRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Number (ARN) of the private CA that issued the permissions. You can find the CA's ARN by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action. This must have the following form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i>\
  \ </code>. </p>\"\n        }\n      ]\n    },\n    \"Principal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principal\"\n        },\n        {\n          \"description\": \"The Amazon Web Services service or identity that will have its CA permissions revoked. At this time, the only valid service principal is <code>acm.amazonaws.com</code> \"\n        }\n      ]\n    },\n    \"SourceAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account that calls this action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"Principal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-permission-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DeletePermissionRequest
---
