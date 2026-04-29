---
description: Represents information about the result of an approval request.
layout: schema
name: ApprovalResult
properties_list:
- description: ''
  name: summary
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-approval-result-schema.json
slug: amazon-codepipeline-approval-result
source_filename: amazon-codepipeline-approval-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-approval-result-schema.json\",\n  \"title\": \"ApprovalResult\",\n  \"description\": \"Represents information about the result of an approval request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApprovalSummary\"\n        },\n        {\n          \"description\": \"The summary of the current status of the approval request.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApprovalStatus\"\n        },\n        {\n          \"description\": \"The response submitted by a reviewer assigned to an approval action request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"summary\",\n    \"status\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-approval-result-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ApprovalResult
---
