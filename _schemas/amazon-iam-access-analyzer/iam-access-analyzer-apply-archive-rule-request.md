---
description: Retroactively applies an archive rule.
layout: schema
name: ApplyArchiveRuleRequest
properties_list:
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: ruleName
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-apply-archive-rule-request-schema.json
slug: iam-access-analyzer-apply-archive-rule-request
source_filename: iam-access-analyzer-apply-archive-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-apply-archive-rule-request-schema.json\",\n  \"title\": \"ApplyArchiveRuleRequest\",\n  \"description\": \"Retroactively applies an archive rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The Amazon resource name (ARN) of the analyzer.\"\n        }\n      ]\n    },\n    \"ruleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the rule to apply.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n    \
  \    {\n          \"description\": \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerArn\",\n    \"ruleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-apply-archive-rule-request-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ApplyArchiveRuleRequest
---
