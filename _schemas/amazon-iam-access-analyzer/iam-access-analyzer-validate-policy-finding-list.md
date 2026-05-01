---
description: ValidatePolicyFindingList schema from AWS IAM Access Analyzer API
layout: schema
name: ValidatePolicyFindingList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-validate-policy-finding-list-schema.json
slug: iam-access-analyzer-validate-policy-finding-list
source_filename: iam-access-analyzer-validate-policy-finding-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-finding-list-schema.json\",\n  \"title\": \"ValidatePolicyFindingList\",\n  \"description\": \"ValidatePolicyFindingList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"findingDetails\",\n      \"findingType\",\n      \"issueCode\",\n      \"learnMoreLink\",\n      \"locations\"\n    ],\n    \"properties\": {\n      \"findingDetails\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"A localized message that explains the finding and provides guidance on how to address it.\"\n          }\n        ]\n      },\n      \"findingType\": {\n        \"allOf\": [\n         \
  \ {\n            \"$ref\": \"#/components/schemas/ValidatePolicyFindingType\"\n          },\n          {\n            \"description\": \"<p>The impact of the finding.</p> <p>Security warnings report when the policy allows access that we consider overly permissive.</p> <p>Errors report when a part of the policy is not functional.</p> <p>Warnings report non-security issues when a policy does not conform to policy writing best practices.</p> <p>Suggestions recommend stylistic improvements in the policy that do not impact access.</p>\"\n          }\n        ]\n      },\n      \"issueCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IssueCode\"\n          },\n          {\n            \"description\": \"The issue code provides an identifier of the issue associated with this finding.\"\n          }\n        ]\n      },\n      \"learnMoreLink\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LearnMoreLink\"\n        \
  \  },\n          {\n            \"description\": \"A link to additional documentation about the type of finding.\"\n          }\n        ]\n      },\n      \"locations\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LocationList\"\n          },\n          {\n            \"description\": \"The list of locations in the policy document that are related to the finding. The issue code provides a summary of an issue identified by the finding.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A finding in a policy. Each finding is an actionable recommendation that can be used to improve the policy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-finding-list-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ValidatePolicyFindingList
---
