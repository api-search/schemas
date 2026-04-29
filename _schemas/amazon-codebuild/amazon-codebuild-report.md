---
description: Information about the results from running a series of test cases during the run of a build project. The test cases are specified in the buildspec for the build project using one or more paths to the test case files. You can specify any type of tests you want, such as unit tests, integration tests, and functional tests.
layout: schema
name: Report
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: reportGroupArn
  type: object
- description: ''
  name: executionId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: expired
  type: object
- description: ''
  name: exportConfig
  type: object
- description: ''
  name: truncated
  type: object
- description: ''
  name: testSummary
  type: object
- description: ''
  name: codeCoverageSummary
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-schema.json
slug: amazon-codebuild-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-schema.json\",\n  \"title\": \"Report\",\n  \"description\": \"Information about the results from running a series of test cases during the run of a build project. The test cases are specified in the buildspec for the build project using one or more paths to the test case files. You can specify any type of tests you want, such as unit tests, integration tests, and functional tests. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the report run. \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportType\"\n        },\n        {\n   \
  \       \"description\": \"<p>The type of the report that was run.</p> <dl> <dt>CODE_COVERAGE</dt> <dd> <p>A code coverage report.</p> </dd> <dt>TEST</dt> <dd> <p>A test report.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The name of the report that was run. \"\n        }\n      ]\n    },\n    \"reportGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the report group associated with this report. \"\n        }\n      ]\n    },\n    \"executionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The ARN of the build run that generated this report. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/ReportStatusType\"\n        },\n        {\n          \"description\": \" The status of this report. \"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time this report run occurred. \"\n        }\n      ]\n    },\n    \"expired\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time a report expires. A report expires 30 days after it is created. An expired report is not available to view in CodeBuild. \"\n        }\n      ]\n    },\n    \"exportConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportExportConfig\"\n        },\n        {\n          \"description\": \" Information about where the raw data used to generate this report was exported.\
  \ \"\n        }\n      ]\n    },\n    \"truncated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" A boolean that specifies if this report run is truncated. The list of test cases is truncated after the maximum number of test cases is reached. \"\n        }\n      ]\n    },\n    \"testSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestReportSummary\"\n        },\n        {\n          \"description\": \" A <code>TestReportSummary</code> object that contains information about this test report. \"\n        }\n      ]\n    },\n    \"codeCoverageSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeCoverageReportSummary\"\n        },\n        {\n          \"description\": \"A <code>CodeCoverageReportSummary</code> object that contains a code coverage summary for this report.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: Report
---
