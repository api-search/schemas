---
description: StartPolicyGenerationResponse schema from AWS IAM Access Analyzer API
layout: schema
name: StartPolicyGenerationResponse
properties_list:
- description: ''
  name: jobId
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-start-policy-generation-response-schema.json
slug: iam-access-analyzer-start-policy-generation-response
source_filename: iam-access-analyzer-start-policy-generation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-start-policy-generation-response-schema.json\",\n  \"title\": \"StartPolicyGenerationResponse\",\n  \"description\": \"StartPolicyGenerationResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The <code>JobId</code> that is returned by the <code>StartPolicyGeneration</code> operation. The <code>JobId</code> can be used with <code>GetGeneratedPolicy</code> to retrieve the generated policies or used with <code>CancelPolicyGeneration</code> to cancel the policy generation request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-start-policy-generation-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: StartPolicyGenerationResponse
---
