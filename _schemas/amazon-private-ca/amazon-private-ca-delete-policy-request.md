---
description: DeletePolicyRequest schema from Amazon Private CA API
layout: schema
name: DeletePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-delete-policy-request-schema.json
slug: amazon-private-ca-delete-policy-request
source_filename: amazon-private-ca-delete-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-policy-request-schema.json\",\n  \"title\": \"DeletePolicyRequest\",\n  \"description\": \"DeletePolicyRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the private CA that will have its policy deleted. You can find the CA's ARN by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action. The ARN value must have the form <code>arn:aws:acm-pca:region:account:certificate-authority/01234567-89ab-cdef-0123-0123456789ab</code>. \"\n        }\n     \
  \ ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-delete-policy-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: DeletePolicyRequest
---
