---
description: Contains the unmodified data for the report. For more information, see .
layout: schema
name: ReportWithRawData
properties_list:
- description: ''
  name: reportArn
  type: object
- description: ''
  name: data
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-with-raw-data-schema.json
slug: amazon-codebuild-report-with-raw-data
source_filename: amazon-codebuild-report-with-raw-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-with-raw-data-schema.json\",\n  \"title\": \"ReportWithRawData\",\n  \"description\": \"Contains the unmodified data for the report. For more information, see .\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the report.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the requested data field from the report.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-with-raw-data-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ReportWithRawData
---
