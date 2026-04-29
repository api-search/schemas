---
description: Describes the certificate extensions to be added to the certificate signing request (CSR).
layout: schema
name: CsrExtensions
properties_list:
- description: ''
  name: KeyUsage
  type: object
- description: ''
  name: SubjectInformationAccess
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-csr-extensions-schema.json
slug: amazon-private-ca-csr-extensions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-csr-extensions-schema.json\",\n  \"title\": \"CsrExtensions\",\n  \"description\": \"Describes the certificate extensions to be added to the certificate signing request (CSR).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyUsage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyUsage\"\n        },\n        {\n          \"description\": \"Indicates the purpose of the certificate and of the key contained in the certificate.\"\n        }\n      ]\n    },\n    \"SubjectInformationAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessDescriptionList\"\n        },\n        {\n          \"description\": \"For CA certificates, provides a path to additional information pertaining to the CA, such as revocation\
  \ and policy. For more information, see <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.2.2\\\">Subject Information Access</a> in RFC 5280.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-csr-extensions-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CsrExtensions
---
