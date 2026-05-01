---
description: ImportCertificateAuthorityCertificateRequest schema from Amazon Private CA API
layout: schema
name: ImportCertificateAuthorityCertificateRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: Certificate
  type: object
- description: ''
  name: CertificateChain
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-import-certificate-authority-certificate-request-schema.json
slug: amazon-private-ca-import-certificate-authority-certificate-request
source_filename: amazon-private-ca-import-certificate-authority-certificate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-import-certificate-authority-certificate-request-schema.json\",\n  \"title\": \"ImportCertificateAuthorityCertificateRequest\",\n  \"description\": \"ImportCertificateAuthorityCertificateRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that was returned when you called <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a>. This must be of the form: </p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i>\
  \ </code> </p>\"\n        }\n      ]\n    },\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBodyBlob\"\n        },\n        {\n          \"description\": \"The PEM-encoded certificate for a private CA. This may be a self-signed certificate in the case of a root CA, or it may be signed by another CA that you control.\"\n        }\n      ]\n    },\n    \"CertificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateChainBlob\"\n        },\n        {\n          \"description\": \"<p>A PEM-encoded file that contains all of your certificates, other than the certificate you're importing, chaining up to your root CA. Your Amazon Web Services Private CA-hosted or on-premises root certificate is the last in the chain, and each certificate in the chain signs the one preceding. </p> <p>This parameter must be supplied when you import a subordinate CA. When you import a root CA, there is no\
  \ chain.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"Certificate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-import-certificate-authority-certificate-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ImportCertificateAuthorityCertificateRequest
---
