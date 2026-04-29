---
description: CreateReportGroupOutput schema from Amazon CodeBuild
layout: schema
name: CreateReportGroupOutput
properties_list:
- description: ''
  name: reportGroup
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-report-group-output-schema.json
slug: amazon-codebuild-create-report-group-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-report-group-output-schema.json\",\n  \"title\": \"CreateReportGroupOutput\",\n  \"description\": \"CreateReportGroupOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroup\"\n        },\n        {\n          \"description\": \" Information about the report group that was created. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-report-group-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateReportGroupOutput
---
