---
description: A filter used to return reports with the status specified by the input <code>status</code> parameter.
layout: schema
name: ReportFilter
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-filter-schema.json
slug: amazon-codebuild-report-filter
source_filename: amazon-codebuild-report-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-filter-schema.json\",\n  \"title\": \"ReportFilter\",\n  \"description\": \" A filter used to return reports with the status specified by the input <code>status</code> parameter. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportStatusType\"\n        },\n        {\n          \"description\": \" The status used to filter reports. You can filter using one status only. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-filter-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ReportFilter
---
