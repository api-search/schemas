---
description: GetReportGroupTrendInput schema from Amazon CodeBuild
layout: schema
name: GetReportGroupTrendInput
properties_list:
- description: ''
  name: reportGroupArn
  type: object
- description: ''
  name: numOfReports
  type: object
- description: ''
  name: trendField
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-get-report-group-trend-input-schema.json
slug: amazon-codebuild-get-report-group-trend-input
source_filename: amazon-codebuild-get-report-group-trend-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-report-group-trend-input-schema.json\",\n  \"title\": \"GetReportGroupTrendInput\",\n  \"description\": \"GetReportGroupTrendInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the report group that contains the reports to analyze.\"\n        }\n      ]\n    },\n    \"numOfReports\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"<p>The number of reports to analyze. This operation always retrieves the most recent reports.</p> <p>If this parameter is omitted, the most recent 100\
  \ reports are analyzed.</p>\"\n        }\n      ]\n    },\n    \"trendField\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupTrendFieldType\"\n        },\n        {\n          \"description\": \"<p>The test report value to accumulate. This must be one of the following values:</p> <dl> <dt>Test reports:</dt> <dd> <dl> <dt>DURATION</dt> <dd> <p>Accumulate the test run times for the specified reports.</p> </dd> <dt>PASS_RATE</dt> <dd> <p>Accumulate the percentage of tests that passed for the specified test reports.</p> </dd> <dt>TOTAL</dt> <dd> <p>Accumulate the total number of tests for the specified test reports.</p> </dd> </dl> </dd> </dl> <dl> <dt>Code coverage reports:</dt> <dd> <dl> <dt>BRANCH_COVERAGE</dt> <dd> <p>Accumulate the branch coverage percentages for the specified test reports.</p> </dd> <dt>BRANCHES_COVERED</dt> <dd> <p>Accumulate the branches covered values for the specified test reports.</p> </dd> <dt>BRANCHES_MISSED</dt> <dd>\
  \ <p>Accumulate the branches missed values for the specified test reports.</p> </dd> <dt>LINE_COVERAGE</dt> <dd> <p>Accumulate the line coverage percentages for the specified test reports.</p> </dd> <dt>LINES_COVERED</dt> <dd> <p>Accumulate the lines covered values for the specified test reports.</p> </dd> <dt>LINES_MISSED</dt> <dd> <p>Accumulate the lines not covered values for the specified test reports.</p> </dd> </dl> </dd> </dl>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportGroupArn\",\n    \"trendField\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-report-group-trend-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: GetReportGroupTrendInput
---
