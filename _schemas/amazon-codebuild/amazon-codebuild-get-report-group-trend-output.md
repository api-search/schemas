---
description: GetReportGroupTrendOutput schema from Amazon CodeBuild
layout: schema
name: GetReportGroupTrendOutput
properties_list:
- description: ''
  name: stats
  type: object
- description: ''
  name: rawData
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-get-report-group-trend-output-schema.json
slug: amazon-codebuild-get-report-group-trend-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-report-group-trend-output-schema.json\",\n  \"title\": \"GetReportGroupTrendOutput\",\n  \"description\": \"GetReportGroupTrendOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stats\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupTrendStats\"\n        },\n        {\n          \"description\": \"Contains the accumulated trend data.\"\n        }\n      ]\n    },\n    \"rawData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupTrendRawDataList\"\n        },\n        {\n          \"description\": \"An array that contains the raw data for each report.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-report-group-trend-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: GetReportGroupTrendOutput
---
