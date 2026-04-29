---
description: DeleteReportGroupInput schema from Amazon CodeBuild
layout: schema
name: DeleteReportGroupInput
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: deleteReports
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-delete-report-group-input-schema.json
slug: amazon-codebuild-delete-report-group-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-report-group-input-schema.json\",\n  \"title\": \"DeleteReportGroupInput\",\n  \"description\": \"DeleteReportGroupInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the report group to delete. \"\n        }\n      ]\n    },\n    \"deleteReports\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>If <code>true</code>, deletes any reports that belong to a report group before deleting the report group. </p> <p>If <code>false</code>, you must delete any reports in the report group. Use <a\
  \ href=\\\"https://docs.aws.amazon.com/codebuild/latest/APIReference/API_ListReportsForReportGroup.html\\\">ListReportsForReportGroup</a> to get the reports in a report group. Use <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/APIReference/API_DeleteReport.html\\\">DeleteReport</a> to delete the reports. If you call <code>DeleteReportGroup</code> for a report group that contains one or more reports, an exception is thrown. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-report-group-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DeleteReportGroupInput
---
