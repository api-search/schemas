---
description: Contains the generated policy details.
layout: schema
name: GeneratedPolicyProperties
properties_list:
- description: ''
  name: isComplete
  type: object
- description: ''
  name: principalArn
  type: object
- description: ''
  name: cloudTrailProperties
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-generated-policy-properties-schema.json
slug: iam-access-analyzer-generated-policy-properties
source_filename: iam-access-analyzer-generated-policy-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-properties-schema.json\",\n  \"title\": \"GeneratedPolicyProperties\",\n  \"description\": \"Contains the generated policy details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isComplete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"This value is set to <code>true</code> if the generated policy contains all possible actions for a service that IAM Access Analyzer identified from the CloudTrail trail that you specified, and <code>false</code> otherwise.\"\n        }\n      ]\n    },\n    \"principalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalArn\"\n        },\n        {\n          \"description\": \"The\
  \ ARN of the IAM entity (user or role) for which you are generating a policy.\"\n        }\n      ]\n    },\n    \"cloudTrailProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudTrailProperties\"\n        },\n        {\n          \"description\": \"Lists details about the <code>Trail</code> used to generated policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"principalArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-generated-policy-properties-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: GeneratedPolicyProperties
---
