---
description: AnalyzedResourcesList schema from AWS IAM Access Analyzer API
layout: schema
name: AnalyzedResourcesList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-analyzed-resources-list-schema.json
slug: iam-access-analyzer-analyzed-resources-list
source_filename: iam-access-analyzer-analyzed-resources-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resources-list-schema.json\",\n  \"title\": \"AnalyzedResourcesList\",\n  \"description\": \"AnalyzedResourcesList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"resourceArn\",\n      \"resourceOwnerAccount\",\n      \"resourceType\"\n    ],\n    \"properties\": {\n      \"resourceArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceArn\"\n          },\n          {\n            \"description\": \"The ARN of the analyzed resource.\"\n          }\n        ]\n      },\n      \"resourceOwnerAccount\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n           \
  \ \"description\": \"The Amazon Web Services account ID that owns the resource.\"\n          }\n        ]\n      },\n      \"resourceType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceType\"\n          },\n          {\n            \"description\": \"The type of resource that was analyzed.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains the ARN of the analyzed resource.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resources-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: AnalyzedResourcesList
---
