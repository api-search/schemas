---
description: ListAccessPreviewFindingsResponse schema from AWS IAM Access Analyzer API
layout: schema
name: ListAccessPreviewFindingsResponse
properties_list:
- description: ''
  name: findings
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-access-preview-findings-response-schema.json
slug: iam-access-analyzer-list-access-preview-findings-response
source_filename: iam-access-analyzer-list-access-preview-findings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-access-preview-findings-response-schema.json\",\n  \"title\": \"ListAccessPreviewFindingsResponse\",\n  \"description\": \"ListAccessPreviewFindingsResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewFindingsList\"\n        },\n        {\n          \"description\": \"A list of access preview findings that match the specified filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"findings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-access-preview-findings-response-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ListAccessPreviewFindingsResponse
---
