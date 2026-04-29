---
description: GetPolicyResponse schema from AWS IAM API
layout: schema
name: GetPolicyResponse
properties_list:
- description: ''
  name: GetPolicyResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-get-policy-response-schema.json
slug: amazon-iam-get-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-policy-response-schema.json\",\n  \"title\": \"GetPolicyResponse\",\n  \"description\": \"GetPolicyResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GetPolicyResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Policy\": {\n          \"$ref\": \"#/components/schemas/Policy\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-get-policy-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: GetPolicyResponse
---
