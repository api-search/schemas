---
description: Represents the output of a <code>PutApprovalResult</code> action.
layout: schema
name: PutApprovalResultOutput
properties_list:
- description: ''
  name: approvedAt
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-approval-result-output-schema.json
slug: amazon-codepipeline-put-approval-result-output
source_filename: amazon-codepipeline-put-approval-result-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-approval-result-output-schema.json\",\n  \"title\": \"PutApprovalResultOutput\",\n  \"description\": \"Represents the output of a <code>PutApprovalResult</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"approvedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp showing when the approval or rejection was submitted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-approval-result-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutApprovalResultOutput
---
