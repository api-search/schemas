---
description: Information about a test report.
layout: schema
name: TestReportSummary
properties_list:
- description: ''
  name: total
  type: object
- description: ''
  name: statusCounts
  type: object
- description: ''
  name: durationInNanoSeconds
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-test-report-summary-schema.json
slug: amazon-codebuild-test-report-summary
source_filename: amazon-codebuild-test-report-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-report-summary-schema.json\",\n  \"title\": \"TestReportSummary\",\n  \"description\": \" Information about a test report. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \" The number of test cases in this <code>TestReportSummary</code>. The total includes truncated test cases. \"\n        }\n      ]\n    },\n    \"statusCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportStatusCounts\"\n        },\n        {\n          \"description\": \" A map that contains the number of each type of status returned by the test results in this <code>TestReportSummary</code>. \"\n        }\n      ]\n\
  \    },\n    \"durationInNanoSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperLong\"\n        },\n        {\n          \"description\": \" The number of nanoseconds it took to run all of the test cases in this report. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"total\",\n    \"statusCounts\",\n    \"durationInNanoSeconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-report-summary-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: TestReportSummary
---
