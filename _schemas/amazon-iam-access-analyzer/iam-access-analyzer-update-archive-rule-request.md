---
description: Updates the specified archive rule.
layout: schema
name: UpdateArchiveRuleRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-update-archive-rule-request-schema.json
slug: iam-access-analyzer-update-archive-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-update-archive-rule-request-schema.json\",\n  \"title\": \"UpdateArchiveRuleRequest\",\n  \"description\": \"Updates the specified archive rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteriaMap\"\n        },\n        {\n          \"description\": \"A filter to match for the rules to update. Only rules that match the filter are updated.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"filter\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-update-archive-rule-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: UpdateArchiveRuleRequest
---
