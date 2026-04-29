---
description: PutPolicyRequest schema from Amazon Private CA API
layout: schema
name: PutPolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Policy
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-put-policy-request-schema.json
slug: amazon-private-ca-put-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-put-policy-request-schema.json\",\n  \"title\": \"PutPolicyRequest\",\n  \"description\": \"PutPolicyRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Number (ARN) of the private CA to associate with the policy. The ARN of the CA can be found by calling the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListCertificateAuthorities.html\\\">ListCertificateAuthorities</a> action.</p> <p/>\"\n        }\n      ]\n    },\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSPolicy\"\n        },\n     \
  \   {\n          \"description\": \"The path and file name of a JSON-formatted IAM policy to attach to the specified private CA resource. If this policy does not contain all required statements or if it includes any statement that is not allowed, the <code>PutPolicy</code> action returns an <code>InvalidPolicyException</code>. For information about IAM policy and statement structure, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html#access_policies-json\\\">Overview of JSON Policies</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-put-policy-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: PutPolicyRequest
---
