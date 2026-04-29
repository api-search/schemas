---
description: BatchGetReportsInput schema from Amazon CodeBuild
layout: schema
name: BatchGetReportsInput
properties_list:
- description: ''
  name: reportArns
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-reports-input-schema.json
slug: amazon-codebuild-batch-get-reports-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-reports-input-schema.json\",\n  \"title\": \"BatchGetReportsInput\",\n  \"description\": \"BatchGetReportsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportArns\"\n        },\n        {\n          \"description\": \" An array of ARNs that identify the <code>Report</code> objects to return. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-reports-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetReportsInput
---
