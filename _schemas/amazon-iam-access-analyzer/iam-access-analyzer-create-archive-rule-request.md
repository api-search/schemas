---
description: Creates an archive rule.
layout: schema
name: CreateArchiveRuleRequest
properties_list:
- description: ''
  name: ruleName
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-create-archive-rule-request-schema.json
slug: iam-access-analyzer-create-archive-rule-request
source_filename: iam-access-analyzer-create-archive-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-archive-rule-request-schema.json\",\n  \"title\": \"CreateArchiveRuleRequest\",\n  \"description\": \"Creates an archive rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the rule to create.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteriaMap\"\n        },\n        {\n          \"description\": \"The criteria for the rule.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ruleName\",\n    \"filter\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-archive-rule-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: CreateArchiveRuleRequest
---
