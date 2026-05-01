---
description: RevokeCertificateRequest schema from Amazon Private CA API
layout: schema
name: RevokeCertificateRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: CertificateSerial
  type: object
- description: ''
  name: RevocationReason
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-revoke-certificate-request-schema.json
slug: amazon-private-ca-revoke-certificate-request
source_filename: amazon-private-ca-revoke-certificate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revoke-certificate-request-schema.json\",\n  \"title\": \"RevokeCertificateRequest\",\n  \"description\": \"RevokeCertificateRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>Amazon Resource Name (ARN) of the private CA that issued the certificate to be revoked. This must be of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code> </p>\"\n        }\n      ]\n    },\n    \"CertificateSerial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String128\"\n   \
  \     },\n        {\n          \"description\": \"<p>Serial number of the certificate to be revoked. This must be in hexadecimal format. You can retrieve the serial number by calling <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_GetCertificate.html\\\">GetCertificate</a> with the Amazon Resource Name (ARN) of the certificate you want and the ARN of your private CA. The <b>GetCertificate</b> action retrieves the certificate in the PEM format. You can use the following OpenSSL command to list the certificate in text format and copy the hexadecimal serial number. </p> <p> <code>openssl x509 -in <i>file_path</i> -text -noout</code> </p> <p>You can also copy the serial number from the console or use the <a href=\\\"https://docs.aws.amazon.com/acm/latest/APIReference/API_DescribeCertificate.html\\\">DescribeCertificate</a> action in the <i>Certificate Manager API Reference</i>. </p>\"\n        }\n      ]\n    },\n    \"RevocationReason\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/RevocationReason\"\n        },\n        {\n          \"description\": \"Specifies why you revoked the certificate.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"CertificateSerial\",\n    \"RevocationReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revoke-certificate-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: RevokeCertificateRequest
---
