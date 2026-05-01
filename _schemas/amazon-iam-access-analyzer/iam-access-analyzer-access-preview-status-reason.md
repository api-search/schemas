---
description: Provides more details about the current status of the access preview. For example, if the creation of the access preview fails, a <code>Failed</code> status is returned. This failure can be due to an internal issue with the analysis or due to an invalid proposed resource configuration.
layout: schema
name: AccessPreviewStatusReason
properties_list:
- description: ''
  name: code
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-access-preview-status-reason-schema.json
slug: iam-access-analyzer-access-preview-status-reason
source_filename: iam-access-analyzer-access-preview-status-reason-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-preview-status-reason-schema.json\",\n  \"title\": \"AccessPreviewStatusReason\",\n  \"description\": \"Provides more details about the current status of the access preview. For example, if the creation of the access preview fails, a <code>Failed</code> status is returned. This failure can be due to an internal issue with the analysis or due to an invalid proposed resource configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewStatusReasonCode\"\n        },\n        {\n          \"description\": \"The reason code for the current status of the access preview.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-preview-status-reason-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: AccessPreviewStatusReason
---
