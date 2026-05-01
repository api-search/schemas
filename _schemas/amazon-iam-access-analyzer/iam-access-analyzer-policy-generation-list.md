---
description: PolicyGenerationList schema from AWS IAM Access Analyzer API
layout: schema
name: PolicyGenerationList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-policy-generation-list-schema.json
slug: iam-access-analyzer-policy-generation-list
source_filename: iam-access-analyzer-policy-generation-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-policy-generation-list-schema.json\",\n  \"title\": \"PolicyGenerationList\",\n  \"description\": \"PolicyGenerationList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"jobId\",\n      \"principalArn\",\n      \"status\",\n      \"startedOn\"\n    ],\n    \"properties\": {\n      \"jobId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/JobId\"\n          },\n          {\n            \"description\": \"The <code>JobId</code> that is returned by the <code>StartPolicyGeneration</code> operation. The <code>JobId</code> can be used with <code>GetGeneratedPolicy</code> to retrieve the generated policies or used with <code>CancelPolicyGeneration</code>\
  \ to cancel the policy generation request.\"\n          }\n        ]\n      },\n      \"principalArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PrincipalArn\"\n          },\n          {\n            \"description\": \"The ARN of the IAM entity (user or role) for which you are generating a policy.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/JobStatus\"\n          },\n          {\n            \"description\": \"The status of the policy generation request.\"\n          }\n        ]\n      },\n      \"startedOn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"A timestamp of when the policy generation started.\"\n          }\n        ]\n      },\n      \"completedOn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\
  \n          },\n          {\n            \"description\": \"A timestamp of when the policy generation was completed.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains details about the policy generation status and properties.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-policy-generation-list-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: PolicyGenerationList
---
