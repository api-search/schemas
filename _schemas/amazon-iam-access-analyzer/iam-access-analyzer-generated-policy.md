---
description: Contains the text for the generated policy.
layout: schema
name: GeneratedPolicy
properties_list:
- description: ''
  name: policy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-generated-policy-schema.json
slug: iam-access-analyzer-generated-policy
source_filename: iam-access-analyzer-generated-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-schema.json\",\n  \"title\": \"GeneratedPolicy\",\n  \"description\": \"Contains the text for the generated policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The text to use as the content for the new policy. The policy is created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreatePolicy.html\\\">CreatePolicy</a> action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: GeneratedPolicy
---
