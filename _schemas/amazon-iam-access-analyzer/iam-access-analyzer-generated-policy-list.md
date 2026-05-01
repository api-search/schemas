---
description: GeneratedPolicyList schema from AWS IAM Access Analyzer API
layout: schema
name: GeneratedPolicyList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-generated-policy-list-schema.json
slug: iam-access-analyzer-generated-policy-list
source_filename: iam-access-analyzer-generated-policy-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-list-schema.json\",\n  \"title\": \"GeneratedPolicyList\",\n  \"description\": \"GeneratedPolicyList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"policy\"\n    ],\n    \"properties\": {\n      \"policy\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The text to use as the content for the new policy. The policy is created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreatePolicy.html\\\">CreatePolicy</a> action.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains the text for the generated policy.\"\n \
  \ }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-list-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: GeneratedPolicyList
---
