---
description: BatchGetReportGroupsOutput schema from Amazon CodeBuild
layout: schema
name: BatchGetReportGroupsOutput
properties_list:
- description: ''
  name: reportGroups
  type: object
- description: ''
  name: reportGroupsNotFound
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-report-groups-output-schema.json
slug: amazon-codebuild-batch-get-report-groups-output
source_filename: amazon-codebuild-batch-get-report-groups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-report-groups-output-schema.json\",\n  \"title\": \"BatchGetReportGroupsOutput\",\n  \"description\": \"BatchGetReportGroupsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroups\"\n        },\n        {\n          \"description\": \" The array of report groups returned by <code>BatchGetReportGroups</code>. \"\n        }\n      ]\n    },\n    \"reportGroupsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupArns\"\n        },\n        {\n          \"description\": \" An array of ARNs passed to <code>BatchGetReportGroups</code> that are not associated with a <code>ReportGroup</code>. \"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-report-groups-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetReportGroupsOutput
---
