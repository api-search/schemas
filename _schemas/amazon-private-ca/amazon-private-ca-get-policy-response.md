---
description: GetPolicyResponse schema from Amazon Private CA API
layout: schema
name: GetPolicyResponse
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-get-policy-response-schema.json
slug: amazon-private-ca-get-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-policy-response-schema.json\",\n  \"title\": \"GetPolicyResponse\",\n  \"description\": \"GetPolicyResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSPolicy\"\n        },\n        {\n          \"description\": \"The policy attached to the private CA as a JSON document.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-get-policy-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: GetPolicyResponse
---
