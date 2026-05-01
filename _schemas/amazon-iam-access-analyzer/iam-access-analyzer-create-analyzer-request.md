---
description: Creates an analyzer.
layout: schema
name: CreateAnalyzerRequest
properties_list:
- description: ''
  name: analyzerName
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: archiveRules
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-create-analyzer-request-schema.json
slug: iam-access-analyzer-create-analyzer-request
source_filename: iam-access-analyzer-create-analyzer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-analyzer-request-schema.json\",\n  \"title\": \"CreateAnalyzerRequest\",\n  \"description\": \"Creates an analyzer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the analyzer to create.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"description\": \"The type of analyzer to create. Only ACCOUNT and ORGANIZATION analyzers are supported. You can create only one analyzer per account per Region. You can create up to 5 analyzers per organization per Region.\"\n        }\n      ]\n  \
  \  },\n    \"archiveRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InlineArchiveRulesList\"\n        },\n        {\n          \"description\": \"Specifies the archive rules to add for the analyzer. Archive rules automatically archive findings that meet the criteria you define for the rule.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to apply to the analyzer.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerName\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-analyzer-request-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: CreateAnalyzerRequest
---
