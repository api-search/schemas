---
description: CreatePermissionRequest schema from Amazon Private CA API
layout: schema
name: CreatePermissionRequest
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
- description: ''
  name: Actions
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-create-permission-request-schema.json
slug: amazon-private-ca-create-permission-request
source_filename: amazon-private-ca-create-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-permission-request-schema.json\",\n  \"title\": \"CreatePermissionRequest\",\n  \"description\": \"CreatePermissionRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the CA that grants the permissions. You can find the ARN by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action. This must have the following form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i>\
  \ </code>. </p>\"\n        }\n      ]\n    },\n    \"Principal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principal\"\n        },\n        {\n          \"description\": \"The Amazon Web Services service or identity that receives the permission. At this time, the only valid principal is <code>acm.amazonaws.com</code>.\"\n        }\n      ]\n    },\n    \"SourceAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the calling account.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionList\"\n        },\n        {\n          \"description\": \"The actions that the specified Amazon Web Services service principal can use. These include <code>IssueCertificate</code>, <code>GetCertificate</code>, and <code>ListPermissions</code>.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"CertificateAuthorityArn\",\n    \"Principal\",\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-permission-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CreatePermissionRequest
---
