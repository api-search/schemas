---
description: ListCertificateAuthoritiesResponse schema from Amazon Private CA API
layout: schema
name: ListCertificateAuthoritiesResponse
properties_list:
- description: ''
  name: CertificateAuthorities
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-list-certificate-authorities-response-schema.json
slug: amazon-private-ca-list-certificate-authorities-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-certificate-authorities-response-schema.json\",\n  \"title\": \"ListCertificateAuthoritiesResponse\",\n  \"description\": \"ListCertificateAuthoritiesResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorities\"\n        },\n        {\n          \"description\": \"Summary information about each certificate authority you have created.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"When the list is truncated, this value is present and should be used for the <code>NextToken</code>\
  \ parameter in a subsequent pagination request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-certificate-authorities-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ListCertificateAuthoritiesResponse
---
