---
description: ValidatePolicyResponse schema from AWS IAM Access Analyzer API
layout: schema
name: ValidatePolicyResponse
properties_list:
- description: ''
  name: findings
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-validate-policy-response-schema.json
slug: iam-access-analyzer-validate-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-response-schema.json\",\n  \"title\": \"ValidatePolicyResponse\",\n  \"description\": \"ValidatePolicyResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidatePolicyFindingList\"\n        },\n        {\n          \"description\": \"The list of findings in a policy returned by IAM Access Analyzer based on its suite of policy checks.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"findings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ValidatePolicyResponse
---
