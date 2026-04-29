---
description: BatchGetReportsOutput schema from Amazon CodeBuild
layout: schema
name: BatchGetReportsOutput
properties_list:
- description: ''
  name: reports
  type: object
- description: ''
  name: reportsNotFound
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-reports-output-schema.json
slug: amazon-codebuild-batch-get-reports-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-reports-output-schema.json\",\n  \"title\": \"BatchGetReportsOutput\",\n  \"description\": \"BatchGetReportsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reports\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reports\"\n        },\n        {\n          \"description\": \" The array of <code>Report</code> objects returned by <code>BatchGetReports</code>. \"\n        }\n      ]\n    },\n    \"reportsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportArns\"\n        },\n        {\n          \"description\": \" An array of ARNs passed to <code>BatchGetReportGroups</code> that are not associated with a <code>Report</code>. \"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-reports-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetReportsOutput
---
