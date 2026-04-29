---
description: GetAccessPreviewResponse schema from AWS IAM Access Analyzer API
layout: schema
name: GetAccessPreviewResponse
properties_list:
- description: ''
  name: accessPreview
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-get-access-preview-response-schema.json
slug: iam-access-analyzer-get-access-preview-response
source_filename: iam-access-analyzer-get-access-preview-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-access-preview-response-schema.json\",\n  \"title\": \"GetAccessPreviewResponse\",\n  \"description\": \"GetAccessPreviewResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPreview\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreview\"\n        },\n        {\n          \"description\": \"An object that contains information about the access preview.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessPreview\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-get-access-preview-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: GetAccessPreviewResponse
---
