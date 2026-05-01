---
description: Contains information about an archive rule.
layout: schema
name: ArchiveRuleSummary
properties_list:
- description: ''
  name: ruleName
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-archive-rule-summary-schema.json
slug: iam-access-analyzer-archive-rule-summary
source_filename: iam-access-analyzer-archive-rule-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-archive-rule-summary-schema.json\",\n  \"title\": \"ArchiveRuleSummary\",\n  \"description\": \"Contains information about an archive rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the archive rule.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteriaMap\"\n        },\n        {\n          \"description\": \"A filter used to define the archive rule.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n    \
  \      \"description\": \"The time at which the archive rule was created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the archive rule was last updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ruleName\",\n    \"filter\",\n    \"createdAt\",\n    \"updatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-archive-rule-summary-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ArchiveRuleSummary
---
