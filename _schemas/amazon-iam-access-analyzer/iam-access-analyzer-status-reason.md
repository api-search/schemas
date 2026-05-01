---
description: Provides more details about the current status of the analyzer. For example, if the creation for the analyzer fails, a <code>Failed</code> status is returned. For an analyzer with organization as the type, this failure can be due to an issue with creating the service-linked roles required in the member accounts of the Amazon Web Services organization.
layout: schema
name: StatusReason
properties_list:
- description: ''
  name: code
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-status-reason-schema.json
slug: iam-access-analyzer-status-reason
source_filename: iam-access-analyzer-status-reason-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-status-reason-schema.json\",\n  \"title\": \"StatusReason\",\n  \"description\": \"Provides more details about the current status of the analyzer. For example, if the creation for the analyzer fails, a <code>Failed</code> status is returned. For an analyzer with organization as the type, this failure can be due to an issue with creating the service-linked roles required in the member accounts of the Amazon Web Services organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReasonCode\"\n        },\n        {\n          \"description\": \"The reason code for the current status of the analyzer.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-status-reason-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: StatusReason
---
