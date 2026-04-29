---
description: GetGeneratedPolicyResponse schema from AWS IAM Access Analyzer API
layout: schema
name: GetGeneratedPolicyResponse
properties_list:
- description: ''
  name: jobDetails
  type: object
- description: ''
  name: generatedPolicyResult
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-get-generated-policy-response-schema.json
slug: iam-access-analyzer-get-generated-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-generated-policy-response-schema.json\",\n  \"title\": \"GetGeneratedPolicyResponse\",\n  \"description\": \"GetGeneratedPolicyResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDetails\"\n        },\n        {\n          \"description\": \"A <code>GeneratedPolicyDetails</code> object that contains details about the generated policy.\"\n        }\n      ]\n    },\n    \"generatedPolicyResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedPolicyResult\"\n        },\n        {\n          \"description\": \"A <code>GeneratedPolicyResult</code> object that contains the generated policies\
  \ and associated details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobDetails\",\n    \"generatedPolicyResult\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-generated-policy-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: GetGeneratedPolicyResponse
---
