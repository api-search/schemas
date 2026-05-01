---
description: Contains the ARN details about the IAM entity for which the policy is generated.
layout: schema
name: PolicyGenerationDetails
properties_list:
- description: ''
  name: principalArn
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-policy-generation-details-schema.json
slug: iam-access-analyzer-policy-generation-details
source_filename: iam-access-analyzer-policy-generation-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-policy-generation-details-schema.json\",\n  \"title\": \"PolicyGenerationDetails\",\n  \"description\": \"Contains the ARN details about the IAM entity for which the policy is generated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM entity (user or role) for which you are generating a policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"principalArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-policy-generation-details-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: PolicyGenerationDetails
---
