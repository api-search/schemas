---
description: CreateReportGroupInput schema from Amazon CodeBuild
layout: schema
name: CreateReportGroupInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: exportConfig
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-report-group-input-schema.json
slug: amazon-codebuild-create-report-group-input
source_filename: amazon-codebuild-create-report-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-report-group-input-schema.json\",\n  \"title\": \"CreateReportGroupInput\",\n  \"description\": \"CreateReportGroupInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupName\"\n        },\n        {\n          \"description\": \" The name of the report group. \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportType\"\n        },\n        {\n          \"description\": \" The type of report group. \"\n        }\n      ]\n    },\n    \"exportConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportExportConfig\"\n        },\n        {\n  \
  \        \"description\": \" A <code>ReportExportConfig</code> object that contains information about where the report group test results are exported. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p> A list of tag key and value pairs associated with this report group. </p> <p>These tags are available for use by Amazon Web Services services that support CodeBuild report group tags.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"exportConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-report-group-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateReportGroupInput
---
