---
description: Contains the text for the generated policy and its details.
layout: schema
name: GeneratedPolicyResult
properties_list:
- description: A <code>GeneratedPolicyProperties</code> object that contains properties of the generated policy.
  name: properties
  type: object
- description: ''
  name: generatedPolicies
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-generated-policy-result-schema.json
slug: iam-access-analyzer-generated-policy-result
source_filename: iam-access-analyzer-generated-policy-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-result-schema.json\",\n  \"title\": \"GeneratedPolicyResult\",\n  \"description\": \"Contains the text for the generated policy and its details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"description\": \"A <code>GeneratedPolicyProperties</code> object that contains properties of the generated policy.\"\n    },\n    \"generatedPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedPolicyList\"\n        },\n        {\n          \"description\": \"The text to use as the content for the new policy. The policy is created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreatePolicy.html\\\">CreatePolicy</a> action.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-result-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: GeneratedPolicyResult
---
