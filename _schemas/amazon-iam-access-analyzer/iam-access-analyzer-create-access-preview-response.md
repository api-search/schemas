---
description: CreateAccessPreviewResponse schema from AWS IAM Access Analyzer API
layout: schema
name: CreateAccessPreviewResponse
properties_list:
- description: ''
  name: id
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-create-access-preview-response-schema.json
slug: iam-access-analyzer-create-access-preview-response
source_filename: iam-access-analyzer-create-access-preview-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-access-preview-response-schema.json\",\n  \"title\": \"CreateAccessPreviewResponse\",\n  \"description\": \"CreateAccessPreviewResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewId\"\n        },\n        {\n          \"description\": \"The unique ID for the access preview.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-access-preview-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: CreateAccessPreviewResponse
---
