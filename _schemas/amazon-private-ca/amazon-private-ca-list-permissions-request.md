---
description: ListPermissionsRequest schema from Amazon Private CA API
layout: schema
name: ListPermissionsRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-list-permissions-request-schema.json
slug: amazon-private-ca-list-permissions-request
source_filename: amazon-private-ca-list-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-permissions-request-schema.json\",\n  \"title\": \"ListPermissionsRequest\",\n  \"description\": \"ListPermissionsRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the private CA to inspect. You can find the ARN by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action. This must be of the form: <code>arn:aws:acm-pca:region:account:certificate-authority/12345678-1234-1234-1234-123456789012</code> You can get a private CA's ARN by running\
  \ the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"When paginating results, use this parameter in a subsequent request after you receive a response with truncated results. Set it to the value of <b>NextToken</b> from the response you just received.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"When paginating results, use this parameter to specify the maximum number of items to return in the response. If additional items exist beyond the number you specify, the <b>NextToken</b> element is sent in the response. Use this <b>NextToken</b> value in a subsequent\
  \ request to retrieve additional items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-permissions-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ListPermissionsRequest
---
