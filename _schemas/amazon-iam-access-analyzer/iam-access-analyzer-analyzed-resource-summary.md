---
description: Contains the ARN of the analyzed resource.
layout: schema
name: AnalyzedResourceSummary
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: resourceOwnerAccount
  type: object
- description: ''
  name: resourceType
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-analyzed-resource-summary-schema.json
slug: iam-access-analyzer-analyzed-resource-summary
source_filename: iam-access-analyzer-analyzed-resource-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resource-summary-schema.json\",\n  \"title\": \"AnalyzedResourceSummary\",\n  \"description\": \"Contains the ARN of the analyzed resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the analyzed resource.\"\n        }\n      ]\n    },\n    \"resourceOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that owns the resource.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\
  \n        },\n        {\n          \"description\": \"The type of resource that was analyzed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"resourceOwnerAccount\",\n    \"resourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resource-summary-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: AnalyzedResourceSummary
---
