---
description: GetPolicyRequest schema from Amazon Private CA API
layout: schema
name: GetPolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-get-policy-request-schema.json
slug: amazon-private-ca-get-policy-request
source_filename: amazon-private-ca-get-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-policy-request-schema.json\",\n  \"title\": \"GetPolicyRequest\",\n  \"description\": \"GetPolicyRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the private CA that will have its policy retrieved. You can find the CA's ARN by calling the ListCertificateAuthorities action. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-policy-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GetPolicyRequest
---
