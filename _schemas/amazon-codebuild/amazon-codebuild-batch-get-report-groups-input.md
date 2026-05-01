---
description: BatchGetReportGroupsInput schema from Amazon CodeBuild
layout: schema
name: BatchGetReportGroupsInput
properties_list:
- description: ''
  name: reportGroupArns
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-report-groups-input-schema.json
slug: amazon-codebuild-batch-get-report-groups-input
source_filename: amazon-codebuild-batch-get-report-groups-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-report-groups-input-schema.json\",\n  \"title\": \"BatchGetReportGroupsInput\",\n  \"description\": \"BatchGetReportGroupsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportGroupArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupArns\"\n        },\n        {\n          \"description\": \" An array of report group ARNs that identify the report groups to return. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportGroupArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-report-groups-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetReportGroupsInput
---
