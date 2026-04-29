---
description: ListPolicyGenerationsResponse schema from AWS IAM Access Analyzer API
layout: schema
name: ListPolicyGenerationsResponse
properties_list:
- description: ''
  name: policyGenerations
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-policy-generations-response-schema.json
slug: iam-access-analyzer-list-policy-generations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-policy-generations-response-schema.json\",\n  \"title\": \"ListPolicyGenerationsResponse\",\n  \"description\": \"ListPolicyGenerationsResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyGenerations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyGenerationList\"\n        },\n        {\n          \"description\": \"A <code>PolicyGeneration</code> object that contains details about the generated policy.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"policyGenerations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-policy-generations-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ListPolicyGenerationsResponse
---
