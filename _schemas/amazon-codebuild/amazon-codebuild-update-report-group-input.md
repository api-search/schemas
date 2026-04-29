---
description: UpdateReportGroupInput schema from Amazon CodeBuild
layout: schema
name: UpdateReportGroupInput
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: exportConfig
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-report-group-input-schema.json
slug: amazon-codebuild-update-report-group-input
source_filename: amazon-codebuild-update-report-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-report-group-input-schema.json\",\n  \"title\": \"UpdateReportGroupInput\",\n  \"description\": \"UpdateReportGroupInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the report group to update. \"\n        }\n      ]\n    },\n    \"exportConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportExportConfig\"\n        },\n        {\n          \"description\": \"<p> Used to specify an updated export type. Valid values are: </p> <ul> <li> <p> <code>S3</code>: The report results are exported to an S3 bucket. </p> </li> <li> <p> <code>NO_EXPORT</code>:\
  \ The report results are not exported. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p> An updated list of tag key and value pairs associated with this report group. </p> <p>These tags are available for use by Amazon Web Services services that support CodeBuild report group tags.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-report-group-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateReportGroupInput
---
