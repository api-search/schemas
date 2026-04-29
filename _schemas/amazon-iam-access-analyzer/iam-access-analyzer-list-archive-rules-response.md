---
description: The response to the request.
layout: schema
name: ListArchiveRulesResponse
properties_list:
- description: ''
  name: archiveRules
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-archive-rules-response-schema.json
slug: iam-access-analyzer-list-archive-rules-response
source_filename: iam-access-analyzer-list-archive-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-archive-rules-response-schema.json\",\n  \"title\": \"ListArchiveRulesResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"archiveRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveRulesList\"\n        },\n        {\n          \"description\": \"A list of archive rules created for the specified analyzer.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"archiveRules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-archive-rules-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ListArchiveRulesResponse
---
