---
description: The response to the request.
layout: schema
name: GetArchiveRuleResponse
properties_list:
- description: Contains information about an archive rule.
  name: archiveRule
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-get-archive-rule-response-schema.json
slug: iam-access-analyzer-get-archive-rule-response
source_filename: iam-access-analyzer-get-archive-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-archive-rule-response-schema.json\",\n  \"title\": \"GetArchiveRuleResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"archiveRule\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"ruleName\",\n        \"filter\",\n        \"createdAt\",\n        \"updatedAt\"\n      ],\n      \"properties\": {\n        \"ruleName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Name\"\n            },\n            {\n              \"description\": \"The name of the archive rule.\"\n            }\n          ]\n        },\n        \"filter\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/FilterCriteriaMap\"\n         \
  \   },\n            {\n              \"description\": \"A filter used to define the archive rule.\"\n            }\n          ]\n        },\n        \"createdAt\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time at which the archive rule was created.\"\n            }\n          ]\n        },\n        \"updatedAt\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time at which the archive rule was last updated.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains information about an archive rule.\"\n    }\n  },\n  \"required\": [\n    \"archiveRule\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-archive-rule-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: GetArchiveRuleResponse
---
