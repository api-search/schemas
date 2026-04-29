---
description: InlineArchiveRulesList schema from AWS IAM Access Analyzer API
layout: schema
name: InlineArchiveRulesList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-inline-archive-rules-list-schema.json
slug: iam-access-analyzer-inline-archive-rules-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-inline-archive-rules-list-schema.json\",\n  \"title\": \"InlineArchiveRulesList\",\n  \"description\": \"InlineArchiveRulesList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"ruleName\",\n      \"filter\"\n    ],\n    \"properties\": {\n      \"ruleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the rule.\"\n          }\n        ]\n      },\n      \"filter\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FilterCriteriaMap\"\n          },\n          {\n            \"description\": \"The condition and values for a criterion.\"\n\
  \          }\n        ]\n      }\n    },\n    \"description\": \"An criterion statement in an archive rule. Each archive rule may have multiple criteria.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-inline-archive-rules-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: InlineArchiveRulesList
---
