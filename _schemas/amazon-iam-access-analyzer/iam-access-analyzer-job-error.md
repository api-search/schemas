---
description: Contains the details about the policy generation error.
layout: schema
name: JobError
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-job-error-schema.json
slug: iam-access-analyzer-job-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-job-error-schema.json\",\n  \"title\": \"JobError\",\n  \"description\": \"Contains the details about the policy generation error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobErrorCode\"\n        },\n        {\n          \"description\": \"The job error code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specific information about the error. For example, which service quota was exceeded or which resource was not found.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-job-error-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: JobError
---
