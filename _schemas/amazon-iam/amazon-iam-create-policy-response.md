---
description: CreatePolicyResponse schema from AWS IAM API
layout: schema
name: CreatePolicyResponse
properties_list:
- description: ''
  name: CreatePolicyResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-create-policy-response-schema.json
slug: amazon-iam-create-policy-response
source_filename: amazon-iam-create-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-policy-response-schema.json\",\n  \"title\": \"CreatePolicyResponse\",\n  \"description\": \"CreatePolicyResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatePolicyResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Policy\": {\n          \"$ref\": \"#/components/schemas/Policy\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-policy-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
title: CreatePolicyResponse
---
